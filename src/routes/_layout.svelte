<script lang="ts">
  import Nav from "../components/Nav.svelte";
  import Foo from "../components/Foo.svelte";
  export let segment;
</script>

<Nav {segment} />

<main>
  <slot />
</main>

<Foo />

<style>
  main {
    height: 100vh;
  }
</style>
