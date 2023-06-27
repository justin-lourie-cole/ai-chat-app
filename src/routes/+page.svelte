<script lang="ts">
	import { useChat } from 'ai/svelte';
	import User from '../components/user.svelte';
	import Bot from '../components/bot.svelte';
	import Input from '../components/input.svelte';

	const { messages, handleSubmit, input } = useChat({
		api: '/chat'
	});
</script>

<div class="relative flex h-full max-w-full flex-1 overflow-hidden">
	<div class="flex h-full max-w-full flex-1 flex-col">
		<main
			class="relative h-full w-full transition-width flex flex-col overflow-auto items-stretch flex-1"
		>
			<div class="absolute right-4 top-2 z-10 hidden flex-col gap-2 md:flex" />
			<div class="flex-1 overflow-hidden">
				<div class="react-scroll-to-bottom--css-zcjlz-79elbk h-full dark:bg-gray-800">
					<div class="react-scroll-to-bottom--css-zcjlz-1n7m0yu">
						<div class="flex flex-col text-sm dark:bg-gray-800">
							{#each $messages as message}
								{#if message.role == 'user'}
									<User {message} />
								{:else}
									<Bot {message} />
								{/if}
							{/each}
							<div class="h-32 md:h-48 flex-shrink-0" />
						</div>
					</div>
				</div>
			</div>
		</main>
	</div>
</div>

<div
	class="absolute bottom-0 left-0 w-full border-t md:border-t-0 dark:border-white/20 md:border-transparent md:dark:border-transparent md:bg-vert-light-gradient bg-white dark:bg-gray-800 md:!bg-transparent dark:md:bg-vert-dark-gradient pt-2 md:pl-2 md:w-[calc(100%-.5rem)]"
>
	<Input {handleSubmit} {input} />
</div>
