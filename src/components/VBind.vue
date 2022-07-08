<script>
import TextBind from './components/TextBind.vue';
export default {
  components : {
    TextBind,
  },
  data() {
    return {
      // bind_url : 'http://www.google.com',
      bind_url : 'http://www.daum.net',
      bind_a : {
        bind_url : 'http://www.daum.net',
        domain_name : 'daum',
      },
      bind_img : {
        bind_src : "https://placeimg.com/100/100/any",
        bind_alt : "image size 100*100",
      }
    }
  }
}
</script>

<template>
  <img v-bind:src="bind_img.bind_src" v-bind:alt="bind_img.bind_alt">
  <a v-bind:href="bind_a.bind_url">{{bind_a.domain_name}}</a>
  <h2 id="title">Hello World</h2>
  <!-- <TextBind /> -->
</template>

<style scoped>
#title {
  color:blueviolet;
  text-align: center;
}
</style>
