<template lang="html">
  <div id="above-navbar">
    <div class="above-navbar-background">
      <div class="section">

        <div class="columns">
          <div class="column is-5 is-offset-2">
            <!-- above-navbar-left -->
            <above-navbar-left />
          </div>

          <div class="column is-offset-2">
            <!-- above-navbar-right -->
            <above-navbar-right />
          </div>
        </div>

        <div class="columns is-centered">
          <div class="column is-12 has-text-centered">
            <!-- above-navbar-bottom -->
            <above-navbar-bottom />
          </div>
        </div>


      </div>
    </div>
  </div>
</template>

<script>
import AboveNavbarLeft from './AboveNavbarLeft'
import AboveNavbarRight from './AboveNavbarRight'
import AboveNavbarBottom from './AboveNavbarBottom'

export default {
  components: {
    AboveNavbarLeft,
    AboveNavbarRight,
    AboveNavbarBottom,
  }
}
</script>

<style lang="scss">
.above-navbar-background{
  background: rgb(30,88,161);
  background: linear-gradient(17deg, rgba(30,88,161,1) 0%, rgba(58,36,89,1) 100%);
}
</style>
