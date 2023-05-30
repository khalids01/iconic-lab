<script>
	import Logo1 from './Logo1.svelte';
</script>

<header class="bg-slate-50/5 shadow-sm backdrop-blur-sm">
	<nav class="container max-w-7xl mx-auto w-full flex justify-between px-4 py-2">
		<a href="/" class="text-xl logo font-bold pt-1"> iconic lab </a>
		<div class="flex gap-6">
			<a href="/generate">Generate</a>
		</div>
		<a class="btn btn-sm variant-ghost-surface px-6" href="/login"> Login </a>
	</nav>
</header>

<style>
	.logo {
		font-size: 20px;
		background: linear-gradient(90deg, #39A2CCDC 0%, #3862E9C4 45%, #9A58F0B6 95%, #9A58F0B6 110%);
		/* background: linear-gradient(90deg, #9A58F0B6 0%, #3862E9C4 45%, #39A2CCDC 95%, #39A2CCDC 110%); */
		color: #292929;
		background-clip: text;
		-webkit-background-clip: text;
		-webkit-text-stroke: 4px transparent;
		letter-spacing: 4px;
		animation: ani 30s ease-in-out infinite;
	}

	@keyframes ani {
            0% {
                background-position: -10% 10%;
				background-size: 100%;
            }

            50% {
                background-position: 100% 10%;
				background-size: 100%;
            }

            100% {
				background-position: 300% 10%;
				background-size: 200%;
            }
        }
</style>
