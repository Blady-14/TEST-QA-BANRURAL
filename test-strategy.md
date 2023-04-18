Dentro del código que se encontraron varios erros en los que se pueden  encontrar 
mal redaccion de como querer que funcionara el programa, 


<script>
  //correccion de definicion
  let randomNumber = (Math.floor(Math.random) * 100) + 1;
  // eliminacion de codigo
  //const ATTEMPS = 5;

  
  function checkGuess() {
// correcion a const
    const userGuess = Number(guessField.value);
    if(guessCount === 1) {
      guesses.textContent = 'Número aleatorio anterior: ';

      // correccion de codigo bien definido 
    if (userGuess === randomNumber) {
          lastResult.textContent = 'Felicidades adivinaste el numero';
          lastResult.style.backgroundColor = 'green';
          lowOrHi.textContent = '';
          setGameOver();
        } else if (guessCount === 10) {
          lastResult.textContent = 'Finalización';
          lowOrHi.textContent = '';
          setGameOver();
        } else {
          lastResult.textContent = 'Incorrecto!';
          lastResult.style.backgroundColor = 'red';
          if(userGuess < randomNumber) {
            lowOrHi.textContent = 'El número es menor' ;
          } else if(userGuess > randomNumber) {
            lowOrHi.textContent = 'El número es mayor';
          }
        }

// se hizo una correccion de buenas prácticas.
