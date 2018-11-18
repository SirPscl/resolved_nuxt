<template>
  <div>
    <nuxt/>
  </div>
</template>

<style>
  html {
    font-family: "Courier New", Courier, monospace;
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
    padding: 20px;
    padding-bottom: 120px;
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
        font-size: 60px !important;
      }
    }

  .links {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    padding: 15px;
    text-align: right;
    font-weight: bold;
  }

  a:link {
    color: #35495e;
    text-decoration: none;
  }

  a:hover {
    color: #3e6d47;
  }

  a:visited {
    color: #35495e;
  }

  a:active {
    color: #35495e;
  }


  .link {
    display: block;
    padding: 7px;
  }

  @font-face {
    font-family: 'augie';
    src: url('/augie.ttf');
  }
</style>
