<script lang="ts">
	import 'tailwindcss/tailwind.css';
	import '@skeletonlabs/skeleton/themes/theme-skeleton.css';
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	import '../app.postcss';
</script>

<header class="">
	<nav class="container max-w-7xl mx-auto w-full flex justify-between">
		<a class="btn btn-sm variant-ghost-surface px-6" href="/login"> Login </a>
	</nav>
</header>

<main class="relative h-full">
	<div class="glowing-bg z-0 absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2" />
	<div class="relative z-10 h-full">
		<slot />
	</div>
</main>

<style lang="postcss">
	.glowing-bg {
		@apply w-80 h-80;
	}
	.glowing-bg {
		@apply absolute z-[-1] rounded-full blur-[150px] transition-all;
		animation: pulse 5s cubic-bezier(0, 0, 0, 0.5) infinite, glow 15s linear infinite;
	}
	@keyframes glow {
		0% {
			@apply bg-primary-400/50;
		}
		33% {
			@apply bg-secondary-400/50;
		}
		66% {
			@apply bg-tertiary-400/50;
		}
		100% {
			@apply bg-primary-400/50;
		}
	}
	@keyframes pulse {
		50% {
			scale: 1.1;
		}
	}
</style>
