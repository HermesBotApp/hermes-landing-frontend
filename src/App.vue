<template>
  <div class="container">
    <div class="branding">
      <h1>The future of <span class="highlight">your Discord bot</span> is on the way !</h1>
      <ul>
        <li><social-link link="https://twitter.com/HermesBotApp"><img src="./assets/icons/twitter.svg" alt="Twitter Logo"></social-link></li>
        <li><social-link link="https://hermesbot.app/discord"><img src="./assets/icons/discord.svg" alt="Discorwd"></social-link></li>
        <li><social-link link="https://github.com/HermesBotApp"><img src="./assets/icons/github.svg" alt="Github Logo"></social-link></li>
      </ul>
    </div>
    
    <img id="logo" src="./assets/hermes-logo.svg" alt="Hermes logo">
  </div>
  <footer>
    Copyright Blueberry-Studio • Made with love by <a href="https://grimille.fr">Grimille</a>
  </footer>
</template>

<script>
import 'normalize.css';
import SocialLink from './components/SocialLink.vue';

export default {
  components: { SocialLink },
  name: 'App',
}
</script>

<style lang="scss">
  * {
        box-sizing: border-box;
  }

  a {
    color:#f5f5f5;
    text-decoration: none;
  }

  body {
    font-family: 'Poppins', sans-serif;
    font-size: 20px;
    background: rgb(38,55,43);
background: linear-gradient(315deg, rgb(28, 39, 31) 0%, rgb(34, 22, 22) 100%);
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 100vh;
    width: 100vw;

    h1 {
      color: #f5f5f5;
      text-transform: uppercase;
      letter-spacing: 1px;
      line-height: 1.2;
      font-size: 2.488rem;
      font-weight: bold;
    }

    .container {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate3d(-50%, -70%, 0);
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 0 2em;
      width: 100%;
      max-width: 960px;
      margin: 0 auto;

      #logo {
        position: relative;
        left: -32px;
        max-width: 450px;
      }

      .branding {
        width: 700px;
        min-width: 250px;
        max-width: 450px;

        ul {
          display: flex;
          justify-content: flex-start;
          list-style-type: none;
          padding: 0;
          margin: 0;

          li:nth-child(2) {
            margin: 0 1em;
          }
        }

        .highlight {
          background: #f5f5f5;
          color: rgb(21,23,25);
        }
      }
    }

    footer {
      position: absolute;
      left: 50%;
      transform: translateX(-50%);
      bottom: 1em;
      text-align: center;
      width: 100%;
      max-width: 960px;
      font-size: 0.694rem;
      color:#f5f5f5;
    }
  }
  @media screen and (max-width: 920px) {
    .container {
      max-width: 740px;
      display: flex;
      flex-direction: column-reverse;
      justify-content: center;
      align-items: center;
    }

    h1 {
      margin-top: 0;
      text-align: center;
    }

    .branding {
      ul {
        justify-content: center !important;
      }
    }

    #logo {
        width: 80% !important;
        left: 0 !important;
    }
  }

  @media screen and (max-width: 420px) {
    body {
      font-size: 16px !important;
    }
    
    .container {
      max-width: 380px !important;
    }

    .branding {
        width: 100% !important;
    }

    h1 {
      font-size: 2.441rem;
    }
  }
</style>
