<script setup>
import Image from './components/Image.vue';
import Expression from './components/Expression.vue';

const title = "This is my title";
const desc = "This is my description";
const descHtml = "<i>This is my description</i>";

const data = {
  title: "Title from object",
  desc: "Description from object"
}

const array = [
  {
    title: "Title from array 1",
    desc: "Description from array 1"
  },
  {
    title: "Title from array 2",
    desc: "Description from array 2"
  }
]

</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <!-- <HelloWorld msg="Vite + Vue" /> -->
  <div class="">
    <h1>{{ title }}</h1>
    <!-- <h1 v-text=title></h1> -->
    <!-- <p>{{ desc }}</p> -->
    <p v-html="descHtml"></p>
  </div>
  <!-- <div class="">
    <h1>{{ data.title }}</h1>
    <p>{{ data.desc }}</p>
  </div>
  <div class="">
    <h1>{{ array[1].title }}</h1>
    <p>{{ array[1].desc }}</p>
  </div> -->
  <!-- <Image/> -->
  <Expression/>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
