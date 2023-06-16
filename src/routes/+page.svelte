<script>
	import Logo1 from '$lib/components/header/Logo1.svelte';
	import heroImg from '$lib/assets/images/hero-image-logos.jpg';
	import { Container, Flex } from '$lib/components/ui';
</script>

<Container size="xl" py='pt-4'>
	<Flex wrap='wrap'>
		<Logo1 />
		<img height={300} width={300} alt='Icons' src={heroImg} />
	</Flex>
</Container>
