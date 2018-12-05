<template lang="html">
  <div id="header">
    <!-- Title -->
    <header-title/>

    <!-- HeaderDescription-->
    <header-description/>

    <!-- HeaderItems -->
    <header-items/>

  </div>
</template>

<script>
import HeaderTitle from './HeaderTitle'
import HeaderDescription from './HeaderDescription'
import HeaderItems from './HeaderItems'

export default {
  components: {
    HeaderTitle,
    HeaderDescription,
    HeaderItems,
  }
}
</script>

<style lang="css">
#header {
  margin-top: 65px;
}
</style>
