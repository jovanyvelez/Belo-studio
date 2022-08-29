<script>
    import src from '../confort.svg'
    import imag1 from '../acompañamiento.svg'
    import imag2 from '../profesionalismo.svg'
</script>

<section class="flex justify-center bg-slate-200 mt-2 mx-5 sm:mx-10 ">
    
    <div class="flex flex-col items-center mx-3 h-20 w-32 sm:h-48 sm:w-48 bg-red-500">
        <img src = {imag1} alt="camera" class="mt-1 h-12 w-12 sm:h-36 sm:w-36">
        <p class="text-white text-sm px-2">Acompañamiento</p>
    </div>
    <div class="flex flex-col items-center h-20 w-18 sm:h-48 sm:w-48 bg-red-500">
        <img {src} alt="camera" class="mt-1 h-12 w-12 sm:h-36 sm:w-36">
        <p class="text-white text-sm px-2">Comodidad</p>
    </div>
    <div class="flex flex-col items-center mx-3 h-20 w-32 sm:h-48 sm:w-48 bg-red-500">
        <img src = {imag2} alt="camera" class="mt-1 h-12 w-12 sm:h-36 sm:w-36">
        <p class="text-white text-sm px-2">Profesionalismo</p>
    </div>
</section>