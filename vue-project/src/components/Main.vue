<script setup lang="ts">
import WorkSedction from './WorkSedction.vue';

const work1 = 
{
  imgUrl: '/ume.jpeg',
  title: 'すごい勇者ゲーム',
  desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。',
};

const works = [
    {
      imgUrl: '/ume.jpeg',
      title: 'タイトル1',
      desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。',
    },
    {
      imgUrl: '/ume.jpeg',
      title: 'タイトル2',
      desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。',
    },
    {
      imgUrl: '/ume.jpeg',
      title: 'タイトル3',
      desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。',
    }
]
console.log('works-----', works)
</script>

<template>
    <main>
        <h2>WORKS</h2>
        <!-- <WorkSedction 
            :imgUrl="work1.imgUrl"
            :title="work1.title"
            :desc="work1.desc"
        /> -->
        <!-- <WorkSedction v-bind="works[0]"/>
        <WorkSedction v-bind="works[1]"/> -->

        <WorkSedction v-for="work in works" v-bind="work"/>
    </main>
</template>