<template>
  <div>
    <nuxt/>
  </div>
</template>

<style>
  html {
    font-family: "Courier New", Courier, monospace;
    font-size: 16px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
  }

  @font-face {
    font-family: 'augie';
    src: url('/augie.woff2') format('woff2');
    font-display: fallback;
  }

  *,
  :before,
  :after {
    /* box-sizing: border-box; */
    margin: 0;
  }

  body {
    background-color: #e5e5e5;
    text-align: center;
  }

  .container {
    padding: 10px;
    height: 100%;
  }

  .site-links {
    margin-top: 40px;
  }

  .site-title h1  {
    font-family: augie, Georgia, Arial;
    font-weight: 400;
    font-size: 5rem;
    line-height: 1;
    padding: 20px 0;
    color: #35495e;
    letter-spacing: 1px;
  }

  .site-description {
    color: #35495e;
    font-weight: bold;
    font-size: 1.4rem;;
    margin: auto;
    max-width: 550px;
  }

  .highlight-text {
    color: #3e8d47;
    white-space: nowrap;
    /* text-decoration: underline; */
  }

  .underline-link:hover {
    color: #35495e;
    text-decoration: underline;
  }

  .link {
    display: block;
  }

  a:link {
    color: #35495e;
    text-decoration: none;
    font-weight: bold;
  }

  a:hover {
    color: #3e8d47;
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

  /* Normal layout */
  @media screen and (min-width: 300px) and (min-height: 400px) {

    .container {
      padding: 10px;
      height: 100%;
    }

    .centered {
      position: fixed;
      right: 20px;
      left: 20px;
      top: 40%;
      -webkit-transform: translateY(-50%);
      -moz-transform: translateY(-50%);
      -ms-transform: translateY(-50%);
      -o-transform: translateY(-50%);
      transform: translateY(-50%);
    }

    .site-links {
      text-align: right;
      position: fixed;
      right: 20px;
      bottom: 20px;
    }

    .site-links {
      margin-top: 0;
      text-align: right;
    }
  }

  /* Large layout */
  @media screen and (min-width: 800px) and (min-height: 500px) {
    .site-title h1 {
      font-size: 6rem !important;
    }
  }


</style>
