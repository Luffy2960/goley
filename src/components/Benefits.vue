<script setup lang="ts">
defineProps<{
  items: string[]
}>()
</script>

<template>
  <section id="benefits" class="section benefits">
    <div class="container">
      <h2>Người dùng nhận được gì?</h2>
      <ul>
        <li v-for="item in items" :key="item">{{ item }}</li>
      </ul>
    </div>
  </section>
</template>
