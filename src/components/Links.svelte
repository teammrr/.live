<script>;
    import Github from "./Github.svelte";
    import Portfolio from "./Portfolio.svelte";
    import TimeTabs from "./TimeTabs.svelte";
    import Hub from "./Hub.svelte"; 
    import BookIt from "./BookIt.svelte";
</script>
<div class="flex items-center justify-center pt-6 ">
    <div class="flex flex-col gap-6 lg:gap-4">
        <div class=" text-zinc-700 flex flex-col lg:flex-row lg:gap-0 flex-wrap gap-6 justify-center">
            <TimeTabs />
            <BookIt />
        </div>
        <div class=" text-zinc-700 flex flex-col lg:flex-row lg:gap-0 flex-wrap gap-6 justify-center">
            <Github />
            <Hub />
            <Portfolio />
        </div>
      </div>
</div>