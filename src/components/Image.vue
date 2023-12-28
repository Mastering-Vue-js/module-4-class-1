<script setup>

// const imgUrl = "https://images.unsplash.com/photo-1682685797406-97f364419b4a?q=80&w=3540&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D";
// const alt = "A girl is standing";

const img = {
    src: "https://images.unsplash.com/photo-1682685797406-97f364419b4a?q=80&w=3540&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    alt: 'A girl is standing'
}

</script>
<template>
    <!-- <img v-bind:src="imgUrl" v-bind:alt="alt"> -->
    <!-- <img :src="imgUrl" :alt="alt"> -->
    <img :src="img.src" :alt="img.alt">
    <!-- <img v-bind="img"> -->
</template>