<script>
    let email= " ";
    let isValid=false;
    function validateEmail(){
      /* const regex= /^[\w-\.]+@[\w-]+\.[a-z]{2,7}$/i;   Expresion regular para validar email*/
       const regex= /[^@ \t\r\n]+@[^@ \t\r\n]+\.[^@ \t\r\n]+/;
        isValid = regex.test(email);
    }

</script>
<div class="container">
    <h2>Input Validación</h2>
    <input type="email" bind:value={email} on:input={validateEmail} placeholder="Correo Electronico">
    <p>{isValid ? 'Email válido' : 'Email no válido'}</p>

</div>