<script>
  let count = $state(0)
  const increment = () => {
    if (count <20 )
      count += 1
    }
    
  
   const decrement = () => {
    if (count >0)
    count -= 1
  }
</script>

<h2>Contador: {count}</h2>

<button onclick={increment}>
  Incrementar
</button>
<button onclick={decrement}>
  Decrementar
</button>

