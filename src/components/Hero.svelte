<script>
    import { onMount } from "svelte"
    import { fade, fly, slide } from "svelte/transition"
    import { cubicInOut } from "svelte/easing"
    import Description from "./Description.svelte";
    import Greeting from "./Greeting.svelte";
    import Links from "./Links.svelte";
    
    let ready = false
    
    function setVh() {
    const vh = window.innerHeight * 0.01
    document.documentElement.style.setProperty("--vh", `${vh}px`)
  }

  onMount(() => {
    setVh()
    window.addEventListener("resize", setVh)
    ready = true
  })
</script>

<main class="font-sans bg-zinc-200 dark:bg-zinc-900">
    <div class="fill-viewport-height flex items-center justify-center">
        {#if ready}
          <div
            transition:fade={{ duration: 500, easing: cubicInOut }} class="w-full text-center py-8">
            <div transition:fly={{ y: 200, duration: 800 }}>
              <Greeting />
              <Description />
              <Links />
            </div>
          </div>
        {/if}
      </div>
</main>

