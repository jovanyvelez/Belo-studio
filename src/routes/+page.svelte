<script>
    import Marquee from 'svelte-fast-marquee';
    import Redes from "../components/Redes.svelte";
    let y;
    $: innerWidth = 0;
</script>

<svelte:window bind:innerWidth />
 
<div class="flex mt-10 ml-3 justify-center flex-wrap">
    <button type="button" class="text-black shadow-sm bg-white border border-gray-300 hover:bg-gray-300  font-extrabold rounded-lg text-sm px-5 py-2.5 mr-2 mb-2">Eventos MY</button>
    <button type="button" class="text-black shadow-sm bg-white border border-gray-300 hover:bg-gray-300  font-extrabold rounded-lg text-sm px-5 py-2.5 mr-2 mb-2">Familia MY</button>
    <button type="button" class="text-black shadow-sm bg-white border border-gray-300 hover:bg-gray-300  font-extrabold rounded-lg text-sm px-5 py-2.5 mr-2 mb-2">Descubre la industria</button>
    <button type="button" class="text-black shadow-sm bg-white border border-gray-300 hover:bg-gray-300  font-extrabold rounded-lg text-sm px-5 py-2.5 mr-2 mb-2">Beneficios</button>
    <button type="button" class="text-black shadow-sm bg-white border border-gray-300 hover:bg-gray-300  font-extrabold rounded-lg text-sm px-5 py-2.5 mr-2 mb-2">Haz parte nuestra</button>
</div>

<div class="fixed bottom-4">
    <Marquee speed={20}>
        <h1 class="text-white text-5xl">
            #Atrevete #MY cree en ti #Realiza tus sueños  #Sin limites
        </h1>
    </Marquee>
</div>

<div class="fixed right-4 top-2/4">
    <Redes {innerWidth}/>
</div>


