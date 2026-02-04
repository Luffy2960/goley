<script setup lang="ts">
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Benefits from './components/Benefits.vue'
import Solution from './components/Solution.vue'
import PainPoints from './components/PainPoints.vue'
import CtaEnd from './components/CtaEnd.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <Header />

  <main>
    <Hero />

    <Benefits
      :items="[
        'Trải nghiệm cuộn mượt trên mobile',
        'Nội dung rõ ràng, dễ đọc',
        'CTA nổi bật, dễ bấm'
      ]"
    />

    <Solution
      description="Bố cục bán hàng mobile-first theo hành vi cuộn tự nhiên."
      :items="[
        'Không nhiễu thông tin',
        'Ưu tiên hành động',
        'Dễ tuỳ biến khi code'
      ]"
    />

    <PainPoints
      :items="[
        'Website mobile khó dùng',
        'Người dùng thoát nhanh',
        'Thiếu điểm nhấn'
      ]"
    />

    <CtaEnd />
  </main>

  <Footer />
</template>
