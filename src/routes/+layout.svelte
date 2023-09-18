<script lang='ts'>
	// The ordering of these imports is critical to your app working properly
	import '../app.postcss';
	
	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
	
	import { DarkMode } from 'flowbite-svelte';
	let btnClass = 'transition text-gray-500 dark:text-gray-400 hover:scale-125 hover:bg-gray-100 dark:hover:bg-gray-700 duration-300 rounded-lg text-xl p-2 ';
	import { autoModeWatcher } from '@skeletonlabs/skeleton';
	
	
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering

	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { AppShell } from '@skeletonlabs/skeleton';
	
	// export const load = ({ url }) => {
		// 	const { pathname } = url
		
		// 	return {
			// 		pathname
			// 	}
			// }
			
			// $: console.log($page.url)
			// export let data
		</script>
		
		<!-- <pre>
			{JSON.stringify($page, null, 2)}
		</pre>
		
		<div class="app">
			
			<main>
				{#key $page.url.pathname}
				<div transition:fly={{ y: 20, duration: 1000 }}>
					<slot/>
				</div>
				
				{/key}
			</main>
			
		</div> -->
		
		
		<!-- App Shell -->
		<AppShell>
			<svelte:fragment slot="header">
			
			<!-- App Bar -->
			<div class="absolute visible right-5 top-5 rounded-lg hover:bg-gray-100 focus:z-10 focus:ring-4 focus:outline-none focus:ring-gray-200 dark:text-gray-400 dark:border-gray-600 dark:hover:bg-gray-700 dark:focus:ring-gray-700 gap-2  transition duration-200  lg:invisible ">
				<DarkMode {btnClass} />
			</div>
			<div class="absolute invisible right-6 top-6 rounded-lg hover:bg-gray-100 focus:z-10 focus:ring-4 focus:outline-none focus:ring-gray-200 dark:text-gray-400 dark:border-gray-600 dark:hover:bg-gray-700 dark:focus:ring-gray-700 gap-2  transition duration-200  lg:visible ">
				<DarkMode {btnClass} />
			</div>
			
		</svelte:fragment>
		<!-- Page Route Content -->
		<slot />
	</AppShell>
	
	<svelte:head>{@html `<script>${autoModeWatcher.toString()} autoModeWatcher();</script>`}</svelte:head>
	