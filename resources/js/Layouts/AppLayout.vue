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
  <div class="card">
    <slot />
  </div>
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

.content {
  width: 100%;
  display: flex;
  justify-content: center; /* center horizontally */
  align-items: center;     /* center vertically */
  min-height: calc(100vh - 70px); /* full viewport minus navbar height */
}

.card {
  background: #f3f4f6; /* gray-100 */
  padding: 40px 30px;
  border-radius: 12px;
  box-shadow: 0 10px 20px rgba(0,0,0,0.1);
  width: 90%;
  max-width: 600px;
  text-align: center;
}

.card {
  background: linear-gradient(135deg, #4f46e5, #3b82f6);
  color: white;
}

.btn {
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
}

.card {
  transform: scale(0.98);
  transition: transform 0.3s ease;
}
.card:hover {
  transform: scale(1);
}

</style>

