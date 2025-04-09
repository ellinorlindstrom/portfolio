<script lang="ts">
	import '../styles/index.css';
	import 'styled-system/css';

	let { children } = $props();
</script>

<div class="layout-container">
	{@render children()}
</div>

