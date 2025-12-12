<script setup>
import { Link } from '@inertiajs/vue3'
</script>

<template>
  <div>

    <!-- NAVBAR -->
    <nav class="navbar">
      <div class="nav-container">
        <h2 class="logo">MV's Website :D</h2>

        <div class="nav-links">
          <Link href="/" class="nav-link">Home</Link>
          <Link href="/about" class="nav-link">About</Link>
          <Link href="/products" class="nav-link">Products</Link>
          <Link href="/contact" class="nav-link">Contact</Link>
        </div>
      </div>
    </nav>

    <!-- MAIN CONTENT -->
    <main class="content">
      <slot />
    </main>

  </div>
</template>

<style scoped>
.navbar {
  background: #1f2937; /* Gray-800 */
  color: white;
  padding: 15px 0;
  margin-bottom: 20px;
}

.nav-container {
  width: 90%;
  max-width: 1200px;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 22px;
  font-weight: bold;
}

.nav-links {
  display: flex;
  gap: 20px;
}

.nav-link {
  text-decoration: none;
  color: #d1d5db; /* Gray-300 */
  font-size: 16px;
  transition: 0.2s ease;
}

.nav-link:hover {
  color: white;
}

.content {
  width: 90%;
  max-width: 1200px;
  margin: auto;
}
</style>
