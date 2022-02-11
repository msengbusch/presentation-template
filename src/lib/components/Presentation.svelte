<script lang="ts">
  import 'reveal.js/dist/reveal.css';
  import 'reveal.js/dist/theme/black.css';

  import { onMount } from 'svelte';

  onMount(async () => {
    // Remember: If using multiple Presentation components multiple RevealStatic objects must be created
    const reveal = (await import('reveal.js')).default;
    await reveal.initialize();
  });
</script>

<div class="reveal">
  <div class="slides">
    <slot />
  </div>
</div>

<style>
  .reveal {
    position: absolute;
  }
</style>
