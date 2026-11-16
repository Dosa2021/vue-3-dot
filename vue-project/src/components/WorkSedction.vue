<script setup>
const props = defineProps({
    imgUrl: String,
    title: String,
    desc: String,
})
</script>

<template>
    <section>
        <img :src="imgUrl" alt="すごい勇者ゲーム">
        <h3>{{ title }}</h3>
        <p>{{ desc }}</p>
    </section>
</template>