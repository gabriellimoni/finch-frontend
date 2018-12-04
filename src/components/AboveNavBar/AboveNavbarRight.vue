<template lang="html">
  <div id="above-navbar-right">
    <div class="box has-background-primary has-text-grey-lighter negative">
      <div class="child">
        <h3 class="title is-4 has-text-grey-lighter">Lorem ipsum dolor sit amet, consectetur.</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="css">
#above-navbar-right{
  right: 0;
  margin-top: 25px;
}

.negative {
  transform: skew(-30deg); /* Padrão */
}
.negative > .child {
  margin-left: 20px;
  transform: skew(30deg); /* Padrão */
}
</style>
