<script setup lang="ts">
import WorkSedction from './WorkSedction.vue';

const work1 = {
  imgUrl: '/ume.jpeg',
  title: 'すごい勇者ゲーム',
  desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。',
};

</script>

<template>
    <main>
        <h2>WORKS</h2>
        <!-- <WorkSedction 
            :imgUrl="work1.imgUrl"
            :title="work1.title"
            :desc="work1.desc"
        /> -->
        <WorkSedction v-bind="work1"/>
    </main>
</template>