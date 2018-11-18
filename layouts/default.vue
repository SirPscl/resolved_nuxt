<template>
  <div>
    <nuxt/>
  </div>
</template>

<style>
  html {
    font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }

  *,
  *:before,
  *:after {
    box-sizing: border-box;
    margin: 0;
  }

  .container {
    padding: 10px;
    padding-bottom: 100px;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    background-color: #e5e5e5;
  }

  .main-title {
    font-family: 'augie', sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    line-height: 1;
    color: #35495e;
    letter-spacing: 1px;
  }

    @media screen and (max-width: 500px) {
      .main-title {
        font-size: 75px !important;
      }
    }

    @media screen and (max-height: 300px) {
      .main-title {
        font-size: 50px !important;
      }

      .links {
        font-size: 1rem !important;
      }
    }

  .links {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    padding-bottom: 25px;
    font-size: 1.2rem;
  }

  a.link:link:nth-of-type(1) {
    color: #3e6d47;
  }

  a.link:link:nth-of-type(2) {
    color: #8f6442;
  }

  .link {
    display: block;
    padding-top: 10px;
  }

  @font-face {
    font-family: 'augie';
    src: url('/augie.ttf');
  }
</style>
