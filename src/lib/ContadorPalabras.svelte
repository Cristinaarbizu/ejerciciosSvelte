<script>
    let count = 0; 
    let words = []; 
    let currentWord = ''; 
  
    // Función para añadir la palabra y actualizar el contador
    function addWord() {
      if (currentWord.trim() !== '') {
        words = [...words, currentWord]; 
        count += 1; 
        currentWord = '';
      }
    }
  </script>
  
  <h2>Contador de Palabras: {count}</h2>
  
  <input
    type="text"
    placeholder="Escribe una palabra"
    bind:value={currentWord}
    on:keypress={(e) => e.key === 'Enter' && addWord()}
  />
  
  <h3>Palabras Insertadas:</h3>
  <ul>
    {#each words as word}
      <li>{word}</li>
    {/each}
  </ul>
  
  
