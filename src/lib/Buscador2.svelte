<script>
    let search ='';
    const items=["Manzana", "Peras", "Fresas", "Kiwi"];

    function filterItems(){
        return items.filter(item =>
            item.toLowerCase().includes(search.toLowerCase())
        );
    }
  </script>
  <div class="conteiner">
    <h2>Buscador</h2>
    <input type="text" bind:value={search} placeholder="Buscar..."/>

  <ul>
  {#each filterItems() as item}
    <li>{item}</li>
  {/each}
  </ul>
</div>