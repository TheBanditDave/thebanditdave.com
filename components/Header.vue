<template>
  <b-navbar
    toggleable="md"
    type="dark"
    variant="dark"
    fixed="top"
    bg-faded>

    <div class="container">
      <nuxt-link to="/">
        <b-navbar-brand href="#">TheBanditDave</b-navbar-brand>
      </nuxt-link>

      <b-navbar-toggle target="nav_collapse"/>

      <b-collapse
        id="nav_collapse"
        is-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">

          <b-nav-item href="#">Blog</b-nav-item>
          <b-nav-item href="#">Resume</b-nav-item>

        </b-navbar-nav>

      </b-collapse>
    </div>
  </b-navbar>
</template>

<script>
export default {
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href: 'https://fonts.googleapis.com/css?family=Freckle+Face'
        }
      ]
    }
  }
}
</script>

<style>
body {
  padding-top: 70px;
}
.navbar-brand {
  color: greenyellow !important;
  font-family: 'Freckle Face', cursive;
  padding-top: unset;
  padding-bottom: unset;
  font-size: 1.7rem;
}

.nav-link {
  color: greenyellow !important;
}

.nav-link:hover {
  color: #fff !important;
}

.bg-faded {
  background-color: transparent;
}

@media (max-width: 768px) {
  .navbar-brand {
    margin-left: 20%;
  }
}
</style>
