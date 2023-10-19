<script>;
    import Github from "./Github.svelte";
    import Portfolio from "./Portfolio.svelte";
    import TimeTabs from "./TimeTabs.svelte";
    import Hub from "./Hub.svelte"; 
    import BookIt from "./BookIt.svelte";
</script>
<div class="flex items-center justify-center pt-6">
    <div class="flex flex-col gap-4">
        <div class="flex text-zinc-700 flex-col space-y-8 sm:flex-row sm:space-y-0">
            <Github />
            <Portfolio />
            <Hub />
            <TimeTabs />
            <BookIt />
        </div>
      </div>
</div>