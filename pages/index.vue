<template>
  <div
    id="content"
    class="container">
    <div class="centered">
      <div class="site-title">
        <h1 id="site-title">Pascal Huber</h1>
      </div>
    </div>
    <div class="site-links">
      <a
        href="http://keyserver.ubuntu.com/pks/lookup?op=get&search=0xe1c57858d90c90a9c532349a54415487b3bc3474"
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
  const fadeIn = (element) => {
    var op = 0;
    var timer = setInterval(() => {
      if (op >= 1.0){
        clearInterval(timer);
      }
      element.style.opacity = op;
      element.style.filter = 'alpha(opacity=' + op * 100 + ")";
      op  += 0.03;
    }, 20);
  }

  window.onNuxtReady((app) => {
    setTimeout(function () {
      fadeIn(document.getElementById("content"));
    }, 100)
  });

  export default {
    data() {
      return {
        structuredData: {
          "@context": "http://schema.org",
          "@type": "Person",
          "name": "Pascal Huber",
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
<style lang="postcss">
  #content {
    opacity: 0;
  }
</style>
