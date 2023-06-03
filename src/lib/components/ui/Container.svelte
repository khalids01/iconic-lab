<script>
	export const size = 'xl';
	export let py = 'py-0';
</script>

<div class={`container ${py} w-full max-w-screen-${size} px-4 lg:px-6 2xl:px-8 relative  mx-auto`}>
	<slot />
</div>
