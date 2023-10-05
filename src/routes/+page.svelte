{#if visible}

<div class="flex items-center justify-center h-screen  ">
	<div class="space-y-10 text-center flex flex-col items-center">
		<div class="flex flex-row anim-title" transition:fly={{ y: 120, duration: 600 }} >
			<h2 class="h2 font-semibold">Hello there, I'm Team</h2>
			<p class="h2 ml-2 transition ease-in-out duration-300 hover:rotate-45 hover:scale-125">👋🏻</p>
		</div>
		
		<div class="anim-buttons" transition:fly={{ y: 120, duration: 600 }}>
			<div id="Btns" class="flex flex-col space-y-8 sm:flex-row sm:space-y-0 ">
				<a href="https://portfolio.teamrr.live" class="flex mx-4 xs:mx-0 justify-center gap-2 px-4 py-2 font-medium transition duration-200 text-gray-900 bg-white border border-gray-200 rounded-xl hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:outline-none focus:ring-gray-200 focus:text-blue-700 dark:bg-zinc-800 dark:text-gray-400 dark:border-zinc-800 dark:hover:text-white dark:hover:bg-gray-700 dark:focus:ring-gray-700"><svg class="w-5 h-6 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="none" viewBox="0 0 20 20">
					<path stroke="currentColor" stroke-linecap="round" stroke-width="2" d="M1 10c1.5 1.5 5.25 3 9 3s7.5-1.5 9-3m-9-1h.01M2 19h16a1 1 0 0 0 1-1V6a1 1 0 0 0-1-1H2a1 1 0 0 0-1 1v12a1 1 0 0 0 1 1ZM14 5V3a2 2 0 0 0-2-2H8a2 2 0 0 0-2 2v2h8Z"/>
				</svg>Portfolio</a>
				<a href="https://github.com/teammrr" class="flex mx-4 xs:mx-0 justify-center gap-2 px-4 py-2 font-medium transition duration-200 text-gray-900 bg-white border border-gray-200 rounded-xl hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:outline-none focus:ring-gray-200 focus:text-blue-700 dark:bg-zinc-800 dark:text-gray-400 dark:border-zinc-800 dark:hover:text-white dark:hover:bg-gray-700 dark:focus:ring-gray-700"><svg class="w-6 h-6 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 16"><path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 4 1 8l4 4m10-8 4 4-4 4M11 1 9 15"/></svg>Github</a>
				
				<a href="https://hub.teamrr.live" class="flex mx-4 xs:mx-0 justify-center gap-2 px-4 py-2 font-medium transition duration-200 text-gray-900 bg-white border border-gray-200 rounded-xl hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:outline-none focus:ring-gray-200 focus:text-blue-700 dark:bg-zinc-800 dark:text-gray-400 dark:border-zinc-800 dark:hover:text-white dark:hover:bg-gray-700 dark:focus:ring-gray-700"><svg class="w-6 h-6 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 19 20">
					<path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M2 9.376v.786l8 3.925 8-3.925v-.786M1.994 14.191v.786l8 3.925 8-3.925v-.786M10 1.422 2 5.347l8 3.925 8-3.925-8-3.925Z"/>
				</svg>
				Hub</a>
				<a href="https://timetabs.teamrr.live" class="flex mx-4 xs:mx-0 justify-center gap-2 px-4 py-2 font-medium transition duration-200 text-gray-900 bg-white border border-gray-200 rounded-xl hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:outline-none focus:ring-gray-200 focus:text-blue-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700 dark:focus:ring-gray-700"><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
					<path stroke-linecap="round" stroke-linejoin="round" d="M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 012.25-2.25h13.5A2.25 2.25 0 0121 7.5v11.25m-18 0A2.25 2.25 0 005.25 21h13.5A2.25 2.25 0 0021 18.75m-18 0v-7.5A2.25 2.25 0 015.25 9h13.5A2.25 2.25 0 0121 11.25v7.5m-9-6h.008v.008H12v-.008zM12 15h.008v.008H12V15zm0 2.25h.008v.008H12v-.008zM9.75 15h.008v.008H9.75V15zm0 2.25h.008v.008H9.75v-.008zM7.5 15h.008v.008H7.5V15zm0 2.25h.008v.008H7.5v-.008zm6.75-4.5h.008v.008h-.008v-.008zm0 2.25h.008v.008h-.008V15zm0 2.25h.008v.008h-.008v-.008zm2.25-4.5h.008v.008H16.5v-.008zm0 2.25h.008v.008H16.5V15z" />
				  </svg>
				  TimeTabs</a>
			</div>
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
