<script>
	/**
	 * @type {any}
	 */
	export let handleSubmit, input;
</script>

<form
	on:submit={handleSubmit}
	class="stretch mx-2 flex flex-row gap-3 last:mb-2 md:mx-4 md:last:mb-6 lg:mx-auto lg:max-w-2xl xl:max-w-3xl"
>
	<div class="relative flex h-full flex-1 items-stretch md:flex-col" role="presentation">
		<div
			class="flex flex-col w-full py-[10px] flex-grow md:py-4 md:pl-4 relative border border-black/10 bg-white dark:border-gray-900/50 dark:text-white dark:bg-gray-700 rounded-xl shadow-xs dark:shadow-xs"
		>
			<input
				bind:value={$input}
				id="prompt-textarea"
				tabindex="0"
				data-id="root"
				placeholder="Send a message"
				class="m-0 w-full resize-none border-0 bg-transparent p-0 pr-10 focus:ring-0 focus-visible:ring-0 dark:bg-transparent md:pr-12 pl-3 md:pl-0"
				style="max-height: 200px; height: 24px; overflow-y: hidden;"
			/><button
				class="absolute p-1 rounded-md md:bottom-3 md:p-2 md:right-3 dark:hover:bg-gray-900 dark:disabled:hover:bg-transparent right-2 disabled:text-gray-400 enabled:bg-brand-purple text-white bottom-1.5 transition-colors disabled:opacity-40"
				><span class="" data-state="closed"
					><svg
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 16 16"
						fill="none"
						class="h-4 w-4 m-1 md:m-0"
						stroke-width="2"
						><path
							d="M.5 1.163A1 1 0 0 1 1.97.28l12.868 6.837a1 1 0 0 1 0 1.766L1.969 15.72A1 1 0 0 1 .5 14.836V10.33a1 1 0 0 1 .816-.983L8.5 8 1.316 6.653A1 1 0 0 1 .5 5.67V1.163Z"
							fill="currentColor"
						/></svg
					></span
				></button
			>
		</div>
	</div>
</form>
