<script setup>
import AppLayout from '@/Layouts/AppLayout.vue'
</script>

<template>
  <AppLayout>
    <h1 class="text-3xl font-bold mb-4">Home!</h1>
    <p class="mb-6">Welcome :DDDD</p>

    <div class="flex gap-3 justify-center">
      <Link href="/about" class="btn">About</Link>
      <Link href="/products" class="btn">Products</Link>
      <Link href="/contact" class="btn">Contact</Link>
    </div>
  </AppLayout>
</template>

<style scoped>
.btn {
  padding: 10px 20px;
  background: #4b5563;
  color: white;
  border-radius: 6px;
  text-decoration: none;
  transition: 0.2s ease;
}
.btn:hover {
  background: #374151;
}
</style>
