<script lang="ts">
  export let handleClick;
  export let color: string; // TODO: Narrow the cardinality of this type.
</script>

<button style="--color: {color}" on:click={handleClick}>Click me!</button>

<style>
  button {
    color: white;
    background-color: var(--color);
  }
</style>
