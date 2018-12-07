<template>
  <div class="container">
    <div class="centered">
      <div class="site-title">
        <h1>Pascal Huber</h1>
      </div>
      <div class="site-description">
        <h2>
          I am a software
          <span class="highlight-text">developer</span>,
          computer science
          <span class="highlight-text">student</span>
          and <span class="highlight-text">co-founder</span> of
          <a
            href="https://quickshift.ch"
            target="_blank">QuickShift</a>.</h2>
      </div>
    </div>
    <div class="site-links">
      <a
        href="http://keys.gnupg.net/pks/lookup?op=vindex&fingerprint=on&search=0x54415487B3BC3474"
        class="link"
        target="_blank">
        [ public key ]
      </a>
      <a
        href="mailto:pascal.huber@resolved.ch"
        class="link">
        [ pascal.huber@resolved.ch ]
      </a>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        structuredData: {
          "@context": "http://schema.org",
          "@type": "Person",
          "name": "Pascal Huber",
          "description": "I am a software developer computer science student and co-founder of QuickShift",
          "email": "pascal.huber@resolved.ch",
          "birthPlace": "St.Gallen",
          "birthDate": "1992-09-09",
          "worksFor": "QuickShift GmbH",
          "alumniOf": "ZHAW School of Engineering",
          "affiliation": "ETH Zürich",
          "homeLocation": "Dübendorf",
          "homeLocation": "Arbon",
          "knowsAbout": "IT Software Computers Development"
          // More structured data...
        },
      }
    },
    head() {
      return {
        __dangerouslyDisableSanitizers: ['script'],
        script: [
          {
            innerHTML: JSON.stringify(this.structuredData),
            type: 'application/ld+json'
          }
        ]
      }
    },
    async asyncData(context) {
    }
  }
</script>
