<template lang="html">
  <div class="navbar-wrapper" ref="navbar">
    <div class="navbar-container">
      <nav
      class="navbar"
      :class="{'is-fixed-top': is_sticky, 'navbar-wrapper': is_sticky}"
      role="navigation"
      aria-label="main navigation">
        <div class="navbar-brand" >
          <a class="navbar-item" href="https://bulma.io">
            <img src="https://bulma.io/images/bulma-logo.png" width="112" height="28">
          </a>

          <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div id="navbarBasicExample" class="navbar-menu">
          <div class="navbar-end" >
            <a class="navbar-item has-text-grey">
              Home
            </a>

            <a class="navbar-item has-text-grey" v-scroll-to="'#header'">
              About
            </a>

            <a class="navbar-item has-text-grey" v-scroll-to="'#achievements-list'">
              Services
            </a>

            <a class="navbar-item has-text-grey">
              Team
            </a>

            <a class="navbar-item has-text-grey">
              Portfolio
            </a>

            <a class="navbar-item has-text-grey">
              Contact
            </a>
          </div>

          <div class="navbar-end">
            <div class="navbar-item">
              <span class="icon"><i class="fab fa-github"></i></span>
            </div>
            <div class="navbar-item has-text-grey">
              <i class="fab fa-twitter"></i>
            </div>
            <div class="navbar-item has-text-grey">
              <i class="fab fa-facebook"></i>
            </div>
            <div class="navbar-item has-text-grey"></div>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      sticky_delta: null,
      is_sticky: false,
    }
  },
  mounted(){
    this.sticky_delta = this.$refs.navbar.offsetTop;
    window.onscroll = () => this.checkNavBar()
  },
  methods: {
    checkNavBar(){
      if (window.pageYOffset > this.sticky_delta) {
        this.is_sticky = true
      } else {
        this.is_sticky = false
      }
    }
  }
}
</script>

<style lang="css" scoped>
.navbar-container{
  margin: 0 80px;
}

.navbar-wrapper{
  border-bottom: 1.5px solid #dadada;
}

.navbar-item {
  flex-grow: 1;
  flex-direction: column;
  justify-content: center;
}
</style>
