<script setup>
import PostItem from '@/components/PostItem.vue'
import MyWrapper from '@/components/MyWrapper.vue'
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
    <MyWrapper>
      <PostItem :post="post" />
    </MyWrapper>
  </div>
</template>
