<script>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
console.log(`New App!`);
export default {
  data() {
    return {
      name : 'John Doe',
      user : {
        name : 'Jine',
        age : 30,
      },
      fruits : ['banana', 'apple', 'mellon'],
      button_html : '<button>v-html</button>',
      button_hack : `<button onclick='document.body.style="background:blue;"'>css hack</button>`,
    }
  }
}
</script>

<template>
  <div v-html="button_hack"></div>
  <div v-html="button_html"></div>
  <div v-text="name"></div>

  <hr>
  <div>{{name}}</div>
  <div>{{user}}, {{user.name}}:{{user.age}}</div>
  <div>array : {{fruits}}, {{fruits[2]}}</div>

</template>

<style scoped>
div {
  margin: 1rem;
  border: 0.2rem solid gray;
}
</style>
