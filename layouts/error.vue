<template>
  <div class="container">
    <div class="centered">
      <div class="site-title">
        <h1
          v-if="error.statusCode === 404"
          class="main-title">
          404
        </h1>
        <h1
          v-else
          class="main-title">
          Error
        </h1>
      </div>
      <div class="site-description">
        <nuxt-link
          to="/"
          class="link">
          [ go back ]
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'NuxtError',
    props: {
      error: {
        type: Object,
        default: null
      }
    }
  }
</script>
