<script>
import Box from "../components/Marquee.svelte"
import logo from '../logo.png'
import Card from "../components/Card.svelte";
	import Marquee from "../components/Marquee.svelte";
</script>

<div>
	<img class="fixed -z-10 left-0 right-0 top-10 bottom-0 mx-auto h-screen" src={logo} alt="">
</div>

<div class="mt-10">
    <div class="flex flex-wrap items-center  justify-around mt-6  "> 
        <Card text1= "Descubre" text2= "La" text3 = "Industria"/>
        <Card text1= "Beneficios"/>
        <Card text1= "Eventos" text2="MY"/>
    </div>
</div>

<Marquee/>

<div class="mt-64 sm:mt-10">
    <div class="flex flex-wrap items-center  justify-around mt-6  "> 
        <Card text1= "Familia" text2= "MY" />
        <Card text1= "Trabaja" text2="con" text3="nosotros"/>
    </div>
</div>