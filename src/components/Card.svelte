<script>
    export let text1;
    export let text2;
    export let text3;
</script>

<div class="flex justify-center flex-col mb-5 text-white text-sm sm:text-sm lg:text-xl
                items-center bg-transparent border-white border-4
                h-24 w-24 sm:h-40 sm:w-40 rounded-3xl
                mr-3">
    {#if text1}
        <h3 class="font-bold">{text1}</h3>
    {/if}

    {#if text2}
        <h3 class="font-bold">{text2}</h3>
    {/if}

    {#if text3}
        <h3 class="font-bold">{text3}</h3>
    {/if}

</div>