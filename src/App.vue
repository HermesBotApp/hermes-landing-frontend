<template>
  <div class="container">
    <h1>The future of your Discord bot is on the way !</h1>
    <img id="logo" src="./assets/hermes-logo.svg" alt="Hermes logo">
    
  </div>
</template>

<script>
import 'normalize.css';

export default {
  name: 'App',
}
</script>

<style lang="scss">
  * {
        box-sizing: border-box;
  }

  body {
    font-family: 'Poppins', sans-serif;
    font-size: 20px;
    background: rgb(21,23,25);
    background: linear-gradient(315deg, rgba(21,23,25,1) 0%, rgba(33,33,33,1) 100%);
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 100vh;
    width: 100vw;

    h1 {
      color: #f5f5f5;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .container {
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 0 2em;

      #logo {
        max-width: 250px;
      }
    }
  }
</style>
