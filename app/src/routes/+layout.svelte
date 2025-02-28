<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<div class="bg-dullWhite">
	{@render children()}
</div>
