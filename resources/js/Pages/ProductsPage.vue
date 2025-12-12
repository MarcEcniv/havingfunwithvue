<script setup>
import AppLayout from '@/Layouts/AppLayout.vue'
</script>

<template>
  <AppLayout>
    <h1 class="text-3xl font-bold mb-4">Products</h1>
    <p class="mb-6">Welcome to the Products page, Lorem ipsum, dolor sit amet consectetur adipisicing elit. Natus, odit accusantium. Sint inventore ut mollitia illum unde? Tempore fugiat fuga eum. Repudiandae minima eveniet labore vero optio sint praesentium? Soluta.</p>

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
