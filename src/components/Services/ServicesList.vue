<template lang="html">
  <div id="services-list" class="section">
    <div class="columns is-centered">
      <div class="column is-9">
        <div class="columns is-centered is-multiline">

          <!-- ServiceItem -->
          <service-item
              v-for="(service, i) of services"
              :key="i"
              :image_source="service.image_source"
              :title="service.title"
              :text="service.text"/>

        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ServiceItem from './ServiceItem'

export default {
  components: {
    ServiceItem,
  },
  data(){
    return {
      services: [],
    }
  },
  created(){
    // ajax
    this.services = [
      {
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'Some fancy <span style="color: #ff4c4c;">colors</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
      },
      {
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'Some fancy <span style="color: #ff4c4c;">colors</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
      },
      {
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'Some fancy <span style="color: #ff4c4c;">colors</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
      },
      {
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'Some fancy <span style="color: #ff4c4c;">colors</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
      },
      {
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'Some fancy <span style="color: #ff4c4c;">colors</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
      },
      {
        image_source: 'https://bulma.io/images/placeholders/128x128.png',
        title: 'Some fancy <span style="color: #ff4c4c;">colors</span>',
        text: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s",
      },
    ]
  }
}
</script>

<style lang="css">
</style>
