{#if visible}

<div class="flex items-center justify-center h-screen  ">
	<div class="space-y-10 text-center flex flex-col items-center">
		<div class="flex flex-col anim-title" transition:fly={{ y: -120, duration: 600 }} >
			<h2 class="h2 font-semibold">Found one of my devices?</h2>
			<h2 class="h2 font-semibold">Contact me here!</h2>
		</div>
        <div class="flex flex-col space-y-4" transition:fly={{ y: -120, duration: 600 }} >
            <!-- <h3 class="h3">Contact Me Here!</h3> -->
            <a href="tel:+66891234545">📱: +66891234545</a>
            <a href="mailto:suteemonv@gmail.com">✉️: suteemonv@gmail.com</a>
        </div>
	</div>
</div>
{/if}

<style lang="postcss">	

</style>

<script>
	import { onMount } from 'svelte';
	import { fly } from 'svelte/transition'
	
	let visible = false
	onMount(() =>{
		visible = true
	})
</script>
