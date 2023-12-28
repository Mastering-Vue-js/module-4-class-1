<script setup>
const number = 1;
const done = true;

const msg = "Vuejs Batch 2";

// const evenOdd = () => {
//     return (number%2) == 0? "Even": "Odd";
// }

const showAlert = () => {
    alert("This is alert!");
}

</script>
<template>
  <p>{{ number % 2 == 0 ? "Even" : "Odd" }}</p>
  <p>{{ done ? "Complete" : "Pending" }}</p>
  <!-- <p>{{ msg }}</p> -->

  <!-- <p class="desc"
  :class="done? 'active': ''">
    {{ msg.split("").reverse().join("") }}
  </p>
  <p class="desc"
    :class="`item-${number}`"
    :id="`item-${number}`"
    :data-attr="number"
    >
    {{ msg }}
  </p> -->

  <p :data-id="number">{{ number }}</p>

  <a href="#" @click.prevent="showAlert()">Click Here</a>

</template>

<style scoped>
p {
  color: blue;
}
p.active {
  color: red;
}
</style>