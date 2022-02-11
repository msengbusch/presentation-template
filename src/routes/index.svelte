<script context="module" lang="ts">
  export const prerender = true;
</script>

<script lang="ts">
  import 'reveal.js/dist/reveal.css';
  import 'reveal.js/dist/theme/black.css';

  import { onMount } from 'svelte';

  onMount(async () => {
    const Reveal = (await import('reveal.js')).default;

    await Reveal.initialize();
  });
</script>

<svelte:head>
  <title>Home</title>
</svelte:head>

<div class="reveal">
  <div class="slides">
    <section>
      <h2>Barebones Presentation</h2>
      <p>
        This example contains the bare minimum includes and markup required to run a reveal.js
        presentation.
      </p>
    </section>
    <section>
      <h2>No Theme</h2>
      <p>There's no theme included, so it will fall back on browser defaults.</p>
    </section>
  </div>
</div>

<style>
  .reveal {
    position: absolute;
  }
</style>
