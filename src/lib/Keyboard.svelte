<script>
  import Letter from "./Letter.svelte";
  let letterSets = [
    ["q", "w", "e", "r", "t", "y", "u", "i", "o", "p"],
    ["a", "s", "d", "f", "g", "h", "j", "k", "l"],
  ];
</script>

<div>
  {#each letterSets as letters}
    {#each letters as letter}
      <Letter {letter} />
    {/each}
    <br />
  {/each}
</div>

<style scoped>
</style>
