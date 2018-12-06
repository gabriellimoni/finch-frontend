<template lang="html">
  <div id="testimonial" class="section has-text-grey-lighter" style="padding-top:4rem">
    <div class="columns is-centered is-centered-mobile" style="margin: auto;">
      <div class="column is-6 is-three-quarters-mobile has-text-centered-mobile is-marginless">
        <blockquote class="content">
          <h3 class="has-text-grey-lighter has-text-centered">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s
          Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s</h3>
        </blockquote>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
#testimonial{
  background: linear-gradient(50deg, rgba(179,55,105,1) 0%, rgba(179,55,105,1) 16%, rgba(37,55,125,1) 100%);
}

blockquote {
  border:none;
  margin-bottom:-30px;
  position: relative;
  margin: 0 auto;
  padding-left: 0.4em;
}

blockquote h3 {
    font-size:21px;
}

blockquote h3:before {
    content: "\201C";
    font-weight: bold;
    font-size:100px;
    color: rgba(0,0,0,0.3);
    position: absolute;
    top: -0.5em;
    left: -0.3em;
    font-family: 'Georgia';
}
blockquote h3:after {
    content: "\201D";
    font-weight: bold;
    font-size:100px;
    color: rgba(0,0,0,0.3);
    position: absolute;
    bottom: -0.8em;
    right: -0.1em;
    font-family: 'Georgia';
}
</style>
