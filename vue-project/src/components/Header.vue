<script setup>
import { ref } from 'vue';

const intro = 'フロントエンドエンジニア見習いです。';
const imgUrl = '/mei_1.jpg';
let count = ref(0);
</script>

<template>
  <header>
    <!-- <img src="/mei_1.jpg" alt="太郎のアイコン"> -->
    <!-- <img v-bind:src="imgUrl" alt="太郎のアイコン"> -->
    <img :src="imgUrl" alt="太郎のアイコン">

    <h1>山田太郎</h1>
    <!-- <p v-text="intro"></p> -->
     <p>{{ intro }}</p>
     <p>{{ intro.length }}</p>
     <button v-on:click="count++">いいね！ {{ count }}</button>
  </header>
</template>

<!-- Note: scopedをつけることで、cssの適用範囲を、このコンポーネントに限定 -->
<style scoped>
header {
    text-align: center;
    width: 100%;
}
header img {
    width: 100%;
}
</style>