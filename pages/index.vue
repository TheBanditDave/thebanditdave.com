<template>
  <div>
    <Header />
    <div class="container content">
      <logo/>
      <h1 class="title">
        thebanditdave.com
      </h1>
      <h2 class="subtitle">
        Portfolio and blog.
      </h2>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Header from '~/components/Header.vue'
/* Need to start building site to replace outdated site. */
export default {
  components: {
    Logo,
    Header
  }
}
</script>

<style>
.container {
  width: 100%;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.content {
  min-height: 100vh;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
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
</style>
