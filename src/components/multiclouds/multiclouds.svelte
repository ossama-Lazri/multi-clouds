<script>
    import Header from "./sections/header.svelte";
    import Services from "./sections/services.svelte";
    import Scroll from "./sections/scroll.svelte";
    import Accordion from "./sections/accordion.svelte";
    import Footer from "./sections/footer.svelte";

    const newMsg = () => {
        alert(`this is used in imported component!`);
    }
</script>

<Header on:click={newMsg} />
<Services />
<Scroll />
<Accordion />
<Footer />