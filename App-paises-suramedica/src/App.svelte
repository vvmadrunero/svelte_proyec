<script>
  import Paises from "./lib/paises.svelte";
  const lista=["colombia","Venezuela","Ecuador"]
</script>
<div class="main">
  {#each lista as pais }
    <div>
      <Paises {pais}/>
    </div>
    {:else}
    no exixten elementos

  {/each}
</div>
<svelte:head>
  <title> Paises de sudamerica</title>
</svelte:head>
<style>
  .main{
    display: grid;
    grid-template-columns: repeat(2,1fr);
        grid-gap:5px;
        grid-auto-rows: minmax(100px, auto);

  }
</style>