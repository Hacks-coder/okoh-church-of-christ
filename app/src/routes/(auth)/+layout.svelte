<script lang="ts">
	import Caption from '../../components/Texts/Caption.svelte';
	import Logo from '../../components/utilities/Logo.svelte';

	let { children } = $props();
</script>

<div class="@container">
		<div class="grid @4xl:grid-cols-2">
		<div class="@container flex flex-col justify-center items-center h-screen gap-5">
			<Caption />
			<Logo />
			{@render children()}
		</div>
		<div class="bg-gold"></div>
	</div>
</div>

