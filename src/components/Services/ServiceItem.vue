<template lang="html">
  <div class="column is-one-third">
    <div class="columns is-marginless">
      <div class="column has-text-right is-3 is-marginless">
        <figure class="image is-64x64" style="margin: auto; margin-bottom:20px;">
          <img :src="image_source">
        </figure>
      </div>

      <div class="column has-text-left has-text-centered-mobile">
        <h3 class="title is-5" v-html="title"></h3>
        <hr style="width: 40%; margin-top:-15px; height: 1.5px;" class="is-hidden-mobile has-background-grey-lighter">
        <p class="is-size-7 has-text-grey-light">{{ text }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['image_source', 'title', 'text']
}
</script>

<style lang="css">
</style>
