<script setup>
const intro = 'フロントエンドエンジニア見習いです。';
</script>

<template>
  <header>
    <img src="/mei_1.jpg" alt="太郎のアイコン">
    <h1>山田太郎</h1>
    <!-- <p v-text="intro"></p> -->
     <p>{{ intro }}</p>
     <p>{{ intro.length }}</p>
  </header>
</template>

<!-- Note: scopedをつけることで、cssの適用範囲を、このコンポーネントに限定 -->
<style scoped>
header {
    background-color: skyblue;
    text-align: center;
    width: 100%;
}
header img {
    width: 100%;
}
</style>