<template>
  <div class="container">
    <div class="centered">
      <div class="site-title">
        <h1>Pascal Huber</h1>
      </div>
      <div class="site-description">
        I am a software
        <span class="highlight-text">developer</span>,
        computer science
        <span class="highlight-text">student</span>
        and <span class="highlight-text">co-founder</span> of
        <a
          class="underline-link"
          href="https://quickshift.ch"
          target="_blank">QuickShift</a>.
      </div>
    </div>
    <div class="site-links">
      <a
        href="https://sks-keyservers.net/pks/lookup?op=get&search=0x54415487b3bc3474"
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
          "description": "I am a software developer computer science student and co-founder of QuickShift.",
          "email": "pascal.huber@resolved.ch",
          "birthDate": "1992-09-09",
          "homeLocation": [
            {
              "@type": "Place",
              "name": "Arbon"
            },{
              "@type": "Place",
              "name": "Dübendorf"
            }
          ],
          "worksFor": "QuickShift GmbH",
          "affiliation": {
            "@type": "CollegeOrUniversity",
            "name": "ETH Zürich"
          },
          "alumniOf": {
            "@type": "CollegeOrUniversity",
            "name": "ZHAW School of Engineering"
          },
          "knowsAbout": "Computer Science"
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
