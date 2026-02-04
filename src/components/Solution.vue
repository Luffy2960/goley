<script setup lang="ts">
defineProps<{
  description: string
  items: string[]
}>()
</script>

<template>
  <section id="solution" class="section solution">
    <div class="container">
      <h2>Giải pháp của Goley</h2>
      <p>{{ description }}</p>
      <ul>
        <li v-for="item in items" :key="item">{{ item }}</li>
      </ul>
    </div>
  </section>
</template>
