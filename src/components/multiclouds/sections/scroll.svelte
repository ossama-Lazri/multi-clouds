<script>
    import cloud2 from '../../../assets/cloud2.svg'

    let faqs = Array(4).fill('Frequently Asked Questions');
</script>

<div id="scroll" class="bg-black px-8 md:py-[1.375rem] py-4 overflow-hidden w-full">
    <div class="inline-flex justify-center items-center gap-8 animate-scroll-right-to-left whitespace-nowrap">
        {#each faqs as faq, index (index)}
            <img src="{cloud2}" alt="">
            <span class="text-[#CEFF1A] md:text-xl font-WorkSansSemiBold leading-7">{faq}</span>
        {/each}
    </div>
</div>