<template lang="html">
  <div id="achievement-item" class="column is-one-quarter">
    <div class="columns is-centered is-vcentered">
      <div class="column">
        <figure class="image is-128x128" style="margin-bottom:20px; margin: auto">
          <img :src="image_source">
        </figure>
      </div>

      <div class="column has-text-left has-text-centered-mobile">
        <h4 class="title has-text-info is-size-1 has-text-weight-bold">{{number}}</h4>
        <h3 class="is-size-5 subtitle has-text-grey-light">{{text}}</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['image_source', 'number', 'text']
}
</script>

<style lang="css">
</style>
