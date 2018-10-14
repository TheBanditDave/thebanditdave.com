<template>
  <b-navbar
    toggleable="md"
    type="dark"
    variant="dark"
    fixed="top"
    bg-faded>

    <div class="container">
      <b-navbar-brand
        nuxt-link
        to="/">TheBanditDave</b-navbar-brand>

      <b-navbar-toggle target="nav_collapse"/>

      <b-collapse
        id="nav_collapse"
        is-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">

          <b-nav-item
            nuxt-link
            to="/blog">BLOG</b-nav-item>
          <b-nav-item
            nuxt-link
            to="/resume">RESUME</b-nav-item>

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
          href: 'https://fonts.googleapis.com/css?family=Knewave|Bangers'
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
  font-family: 'Bangers', cursive;
  padding-top: unset;
  padding-bottom: unset;
  font-size: 1.7rem;
}

.nav-link {
  color: greenyellow !important;
  font-family: 'Knewave', cursive;
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
