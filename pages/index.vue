<template>
  <section class="container">
    <div>
      <h1 class="main-title">Pascal Huber</h1>
      <div class="links">
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
