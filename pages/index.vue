<template>
  <section class="container">
    <div>
      <h1 class="title">Pascal Huber</h1>
      <div class="links">
        <a
          href="mailto:pascal.huber@resolved.ch"
          class="link"
          target="_blank">
          pascal.huber@resolved.ch
        </a>
        <a
          href="https://pgp.mit.edu/pks/lookup?op=vindex&fingerprint=on&search=0x54415487B3BC3474"
          class="link"
          target="_blank">
          public key
        </a>
        <!-- <a
             href="/cv_pascal_huber.pdf"
             class="link"
             target="_blank">
             curriculum vitae
             </a> -->
        <!-- <a
             href="https://github.com/sirpscl"
             target="_blank"
             class="button--grey">
             <fa :icon="faGithub" /> GitHub
             </a> -->
        <!-- <a
             href="https://quickshift.ch"
             target="_blank">
             <img
             class="svg-inline--fa fa-github fa-w-16"
             src="~/assets/quickshift_i.svg">
             QuickShift
             </a> -->
      </div>
    </div>
  </section>
</template>

<script>
  import { faGithub } from '@fortawesome/free-brands-svg-icons'
  import { faKey, faEnvelope, faFileContract } from '@fortawesome/free-solid-svg-icons'

  export default {
    computed: {
      faGithub() {
        return faGithub
      },
      faKey() {
        return faKey
      },
      faEnvelope() {
        return faEnvelope
      },
      faFileContract() {
        return faFileContract
      }
    }
  }
</script>

<style>

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

  .title {
    font-family: 'augie', sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    line-height: 1;
    color: #35495e;
    letter-spacing: 1px;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  .links {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    padding-bottom: 15px;
  }

  a.link:link:nth-of-type(1) {
    color: #a7001e;
  }

  a.link:link:nth-of-type(2) {
    color: #3e5d47;
  }

  a.link:link:nth-of-type(3) {
    color: #76420c;
  }

  /* @media screen and (max-width: 500px) {
     } */

  .link {
    display: block;
    padding-top: 5px;
  }

  @font-face {
    font-family: 'augie';
    src: url('/augie.ttf');
  }

</style>
