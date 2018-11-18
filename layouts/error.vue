<template>
  <div class="container">
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
    <div class="links">
      <nuxt-link
        to="/"
        class="link">
        [ back to safety ]
      </nuxt-link>
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
