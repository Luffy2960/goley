<script setup lang="ts">
defineProps<{
  items: string[]
}>()
</script>

<template>
  <section class="section pain-points">
    <div class="container">
      <h2>Vấn đề thường gặp</h2>
      <ul>
        <li v-for="item in items" :key="item">{{ item }}</li>
      </ul>
    </div>
  </section>
</template>
