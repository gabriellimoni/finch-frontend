<template lang="html">
  <div id="header-items">

    <loading v-if="loading"/>

    <div class="columns is-centered has-text-centered is-multiline">
      <div class="column is-one-third" v-for="(about, i) of about_items" :key="i">
        <div class="section">
          <figure class="image is-128x128" style="margin: auto; margin-bottom:20px;">
            <img :src="about.image_source">
          </figure>

          <h4 class="is-size-5 has-text-grey" v-html="about.title"></h4>

          <div class="columns is-centered has-text-center" style="margin-top: 10px;">
            <div class="column is-6">
              <p class="is-size-7 has-text-grey-light" v-html="about.text"></p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Loading from './../../Loading'

export default {
  components: {
    Loading
  },
  created(){
    // pega os dados via vue-resource
    /*
    this.$http.get(URL)
      .then(res => {
        this.about_items = res.data
      })
    */

    setInterval(()=>{
      this.about_items = [{
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'Some fancy <span style="color: #ff4c4c;">colors</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry"
      },
      {
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'Enough <span style="color: #ff4c4c;">coffe breaks</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry"
      },
      {
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'A little bit of <span style="color: #ff4c4c;">magic</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry"
      }]

      this.loading = false; // fake loading
    }, 1500)
  },
  data(){
    return {
      loading: true, // fake loading
      about_items: []
    }
  }
}
</script>

<style lang="css">
#header-items{
  margin-top: 0;
}
</style>
