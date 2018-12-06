<template lang="html">
  <div id="achievements-list">

    <div class="container">
      <div class="columns is-multiline">
        <!-- AchievementItem -->
        <achievement-item
            v-for="(a, i) of achievements"
            :key="i"
            :image_source="a.image_source"
            :number="a.number"
            :text="a.text"/>
      </div>
    </div>

  </div>
</template>

<script>
import AchievementItem from './AchievementItem'

export default {
  components: {
    AchievementItem,
  },
  data(){
    return {
      achievements: [
        {
          image_source: 'https://bulma.io/images/placeholders/128x128.png',
          number: 1000,
          text: 'Empty cups',
        },
        {
          image_source: 'https://bulma.io/images/placeholders/128x128.png',
          number: 110,
          text: 'Happy clients',
        },
        {
          image_source: 'https://bulma.io/images/placeholders/128x128.png',
          number: 25,
          text: 'BBQ meetings',
        },
        {
          image_source: 'https://bulma.io/images/placeholders/128x128.png',
          number: 29,
          text: 'Cocktail parties',
        },
      ]
    }
  }
}
</script>

<style lang="css">
#achievements-list{
  background-color: #ebebeb;
  padding: 40px 0;
}
</style>
