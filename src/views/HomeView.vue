<script setup>
import PostItem from '@/components/PostItem.vue'

const posts = [
  {
    id: 1,
    title: 'This is great!',
    body: 'telaktlaek akjsakldj adjaow 9idjaw d',
    author: 'Jogn Doe',
    created_at: '11/05/2023',
    is_saved: false
  },
  {
    id: 2,
    title: 'This is great!2',
    body: 'telaktlaek akjsakldj adjaow 9idjaw d2',
    author: 'Jogn Doe2',
    created_at: '12/05/2023',
    is_saved: false
  },
  {
    id: 3,
    title: 'This is great!3',
    body: 'telaktlaek akjsakldj adjaow 9idjaw d3',
    author: 'Jogn Doe3',
    created_at: '13/05/2023',
    is_saved: false
  },
  {
    id: 4,
    title: 'This is great!4',
    body: 'telaktlaek akjsakldj adjaow 9idjaw d4',
    author: 'Jogn Doe4',
    created_at: '14/05/2023',
    is_saved: false
  }
]
</script>

<template>
  <div v-for="post in posts" :key="post.id">
    <div class="wrapper">
      <PostItem :post="post" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.wrapper {
  margin: 2rem;
  background: #fff;
  box-shadow:
    rgba(0, 0, 0, 0.1) 0px 10px 15px -3px,
    rgba(0, 0, 0, 0.05) 0px 4px 6px -2px;
  margin-bottom: 2rem;
  border-radius: 1rem;
  overflow: hidden;
}
</style>
