<script>
export default {
  components : {
  },
  data() {
    return {
      fruits: ['Apple','Banana', 'Orange', 'Apple'],
      user : {
        name : 'jain',
        age : 10,
        city: 'Dallas'
      }
    }
  }
}
</script>

<template>
  <ul>
    <template v-for="(value, key, index) in user" :key="index">
      <li>{{index}}, {{key}}, {{value}}</li>
    </template>
  </ul>
  <ul>
    <template v-for="(fruit, index) in fruits" :key="index">
      <li>{{index}}, {{fruit}}</li>
    </template>
  </ul>
</template>

<style>
</style>
