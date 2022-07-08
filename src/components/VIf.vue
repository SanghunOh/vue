<script>
import TextBind from './components/TextBind.vue';
// import VBind from './components/VBind.vue';

export default {
  components : {
    TextBind,
    // VBind,
  },
  data() {
    return {
      isActive : false,
      user : {
        name : 'jain',
        age : 10
      }
    }
  }
}
</script>

<template>
  <input type="text" name="" id="" v-model="user.age"> {{user.age}}
  <h2 v-if="user.age > 18">Adult {{user.name}}</h2>
  <h2 v-else-if="user.age > 14">Teenager {{user.name}}</h2>
  <h2 v-else>Child {{user.name}}</h2>

  <hr>
  <template v-if="isActive">
    <h2>Hello World!</h2>
    <hr>
  </template>
  <template v-else>
    <h2>Goodbye World!</h2>
  </template>

    <!-- <h2 v-if="isActive">Hello World!</h2>
    <h2 v-else>Goodbye World!</h2> -->
</template>

<style>
</style>
