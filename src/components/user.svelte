<script>
	/**
	 * @type {{ content: any; }}
	 */
	export let message;
</script>

<div
	class="group w-full text-gray-800 dark:text-gray-100 border-b border-black/10 dark:border-gray-900/50 dark:bg-gray-800"
>
	<div
		class="flex p-4 gap-4 text-base md:gap-6 md:max-w-2xl lg:max-w-[38rem] xl:max-w-3xl md:py-6 lg:px-0 m-auto"
	>
		<div class="flex-shrink-0 flex flex-col relative items-end">
			<div class="w-[30px]">
				<div class="relative flex">
					<span
						style="box-sizing: border-box; display: inline-block; overflow: hidden; width: initial; height: initial; background: none; opacity: 1; border: 0px; margin: 0px; padding: 0px; position: relative; max-width: 100%;"
						><span
							style="box-sizing: border-box; display: block; width: initial; height: initial; background: none; opacity: 1; border: 0px; margin: 0px; padding: 0px; max-width: 100%;"
							><img
								alt=""
								aria-hidden="true"
								src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%2738%27%20height=%2738%27/%3e"
								style="display: block; max-width: 100%; width: initial; height: initial; background: none; opacity: 1; border: 0px; margin: 0px; padding: 0px;"
							/></span
						><img
							alt="User"
							srcset="/_next/image?url=https%3A%2F%2Fs.gravatar.com%2Favatar%2F32855c9c69add5a2e0be9db720413e00%3Fs%3D480%26r%3Dpg%26d%3Dhttps%253A%252F%252Fcdn.auth0.com%252Favatars%252Fjc.png&amp;w=48&amp;q=75 1x, /_next/image?url=https%3A%2F%2Fs.gravatar.com%2Favatar%2F32855c9c69add5a2e0be9db720413e00%3Fs%3D480%26r%3Dpg%26d%3Dhttps%253A%252F%252Fcdn.auth0.com%252Favatars%252Fjc.png&amp;w=96&amp;q=75 2x"
							src="/_next/image?url=https%3A%2F%2Fs.gravatar.com%2Favatar%2F32855c9c69add5a2e0be9db720413e00%3Fs%3D480%26r%3Dpg%26d%3Dhttps%253A%252F%252Fcdn.auth0.com%252Favatars%252Fjc.png&amp;w=96&amp;q=75"
							decoding="async"
							data-nimg="intrinsic"
							class="rounded-sm"
							style="position: absolute; inset: 0px; box-sizing: border-box; padding: 0px; border: none; margin: auto; display: block; width: 0px; height: 0px; min-width: 100%; max-width: 100%; min-height: 100%; max-height: 100%;"
						/></span
					>
				</div>
			</div>
			<div
				class="text-xs flex items-center justify-center gap-1 invisible absolute left-0 top-2 -ml-4 -translate-x-full group-hover:visible !invisible"
			>
				<button class="dark:text-white disabled:text-gray-300 dark:disabled:text-gray-400"
					><svg
						stroke="currentColor"
						fill="none"
						stroke-width="1.5"
						viewBox="0 0 24 24"
						stroke-linecap="round"
						stroke-linejoin="round"
						class="h-3 w-3"
						height="1em"
						width="1em"
						xmlns="http://www.w3.org/2000/svg"><polyline points="15 18 9 12 15 6" /></svg
					></button
				><span class="flex-grow flex-shrink-0">1 / 1</span><button
					class="dark:text-white disabled:text-gray-300 dark:disabled:text-gray-400"
					><svg
						stroke="currentColor"
						fill="none"
						stroke-width="1.5"
						viewBox="0 0 24 24"
						stroke-linecap="round"
						stroke-linejoin="round"
						class="h-3 w-3"
						height="1em"
						width="1em"
						xmlns="http://www.w3.org/2000/svg"><polyline points="9 18 15 12 9 6" /></svg
					></button
				>
			</div>
		</div>
		<div class="relative flex w-[calc(100%-50px)] flex-col gap-1 md:gap-3 lg:w-[calc(100%-115px)]">
			<div class="flex flex-grow flex-col gap-3">
				<div
					class="min-h-[20px] flex items-start overflow-x-auto whitespace-pre-wrap break-words flex-col gap-4"
				>
					<div class="empty:hidden">{message.content}</div>
				</div>
			</div>
			<div
				class="text-gray-400 flex self-end lg:self-center justify-center mt-2 gap-2 md:gap-3 lg:gap-1 lg:absolute lg:top-0 lg:translate-x-full lg:right-0 lg:mt-0 lg:pl-2 visible"
			>
				<button
					class="p-1 rounded-md hover:bg-gray-100 hover:text-gray-700 dark:text-gray-400 dark:hover:bg-gray-700 dark:hover:text-gray-200 disabled:dark:hover:text-gray-400 md:invisible md:group-hover:visible"
					><svg
						stroke="currentColor"
						fill="none"
						stroke-width="2"
						viewBox="0 0 24 24"
						stroke-linecap="round"
						stroke-linejoin="round"
						class="h-4 w-4"
						height="1em"
						width="1em"
						xmlns="http://www.w3.org/2000/svg"
						><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7" /><path
							d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"
						/></svg
					></button
				>
			</div>
			<div class="flex justify-between lg:block" />
		</div>
	</div>
</div>
