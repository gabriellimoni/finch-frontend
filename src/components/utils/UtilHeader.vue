<template lang="html">
  <div class="has-centered-text">
    <h1 class="title is-3">{{ title }}</h1>
    <h2 class="subtitle is-4 has-text-grey-light">{{ subtitle }}</h2>
    <hr style="margin: auto; width: 8%; margin-top:0px" class="has-background-grey-lighter">
  </div>
</template>

<script>
export default {
  props: ['title', 'subtitle']
}
</script>

<style lang="css">
</style>
