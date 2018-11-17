<template>
  <section class="container">
    <div>
      <!-- <logo/> -->
      <h1 class="title">Pascal Huber</h1>
      <div class="links">
        <a
          href="http://pgp.mit.edu:11371/pks/lookup?op=get&search=0xE493B06DD070AFC8"
          target="_blank"
          class="main-link button--grey">
          <fa :icon="faKey" /> Public Key
        </a>
        <br>
        <a
          href="/cv_pascal_huber.pdf"
          target="_blank"
          class="main-link button--grey">
          <fa :icon="faFileContract" /> Curriculum Vitae
        </a>
        <br>
        <!-- <a
             href="https://github.com/sirpscl"
             target="_blank"
             class="button--grey">
             <fa :icon="faGithub" /> GitHub
             </a> -->
        <a
          href="https://quickshift.ch"
          target="_blank"
          class="main-link button--grey">
          <img
            class="svg-inline--fa fa-github fa-w-16"
            src="~/assets/quickshift_i.svg">
          QuickShift
        </a>
        <br>
        <a
          href="mailto:pascal.huber@resolved.ch"
          target="_blank"
          class="main-link button--grey">
          <fa :icon="faEnvelope" /> E-Mail
        </a>
      </div>
    </div>
  </section>
</template>

<script>
  import Logo from '~/components/Logo.vue'
  import { faGithub } from '@fortawesome/free-brands-svg-icons'
  import { faKey, faEnvelope, faFileContract } from '@fortawesome/free-solid-svg-icons'

  export default {
    components: {
      Logo
    },
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
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    background-color: #eee;
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
    padding-top: 15px;
  }

  .main-link {
    width: 200px;
    line-height: 2;
    margin: 10px;
  }

  @font-face {
    font-family: 'augie';
    src: url('/augie.ttf');
  }

</style>
