<script lang="ts">
  import Presentation from '$lib/components/Presentation.svelte';
  import Barebone from './slides/Barebone.svelte';
  import Theme from './slides/Theme.svelte';
</script>

<svelte:head>
  <title>Home</title>
</svelte:head>

<Presentation>
  <Barebone />
  <Theme />
</Presentation>
