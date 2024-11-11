<script>
    let isDarkMode = false;
    function toggleTheme() {
      isDarkMode = !isDarkMode;
    }
  </script>
  
  <style>
    .dark-mode {
      background-color: black;
      color: aliceblue;
    }
  
    .light-mode {
      background-color: white;
      color: black;
    }
  </style>
  
  <div class="container" class:dark-mode={isDarkMode} class:light-mode={!isDarkMode}>
    <div>
      <button on:click={toggleTheme}>
        Cambiar a {isDarkMode ? 'Modo claro' : 'Modo Oscuro'}
      </button>
      <h2>Esto es un ejemplo de tema {isDarkMode ? 'Oscuro' : 'Claro'}</h2>
    </div>
  </div>
  