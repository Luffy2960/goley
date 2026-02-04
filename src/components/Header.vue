<script setup lang="ts">
interface NavItem {
  label: string
  href: string
}

const nav: NavItem[] = [
  { label: 'Trang chủ', href: '#home' },
  { label: 'Giải pháp', href: '#solution' },
  { label: 'Lợi ích', href: '#benefits' },
  { label: 'Liên hệ', href: '#contact' },
]
</script>

<template>
  <header class="header">
    <div class="container header-inner">
      <div class="logo">Goley</div>

      <nav class="nav">
        <ul>
          <li v-for="item in nav" :key="item.href">
            <a :href="item.href">{{ item.label }}</a>
          </li>
        </ul>
      </nav>

      <button class="menu-toggle">☰</button>
    </div>
  </header>
</template>
