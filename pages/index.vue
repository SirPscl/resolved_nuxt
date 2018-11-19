<template>
  <div class="container">
    <div class="centered">
      <div class="site-title">
        <h1>Pascal Huber</h1>
      </div>
      <div class="site-description">
        <h2>I am a software <span class="highlight-text">developer</span>, computer science <span class="highlight-text">student</span> and <span class="highlight-text">co-founder</span> of QuickShift LLC.</h2>
      </div>
    </div>
    <div class="site-links">
      <a
        href="https://pgp.mit.edu/pks/lookup?op=vindex&fingerprint=on&search=0x54415487B3BC3474"
        class="link"
        target="_blank">
        [ public key ]
      </a>
      <a
        href="mailto:pascal.huber@resolved.ch"
        class="link"
        target="_blank">
        [ pascal.huber@resolved.ch ]
      </a>
    </div>
  </div>
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
