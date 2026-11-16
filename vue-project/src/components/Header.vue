<template>
  <header>
    <img src="/mei_1.jpg" alt="太郎のアイコン">
    <h1>山田太郎</h1>
    <p>Webデザイナー見習いです</p>
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