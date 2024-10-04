<!-- HeroSection.vue -->
<template>
    <section class="relative h-screen flex items-center justify-center bg-gradient-to-r from-purple-500 to-indigo-500">
      <div class="bg-white/20 backdrop-blur-md p-10 rounded-lg text-center max-w-2xl">
        <h1 class="text-4xl font-bold text-white mb-6">Prepare to Succeed in Competitive Programming</h1>
        <p class="text-white text-lg mb-8">
          Join thousands of coders improving their algorithmic skills with our structured guide.
        </p>
        <button
          @click="scrollToStart"
          class="px-6 py-3 bg-indigo-500 text-white font-semibold rounded-lg shadow-lg transition hover:bg-indigo-700"
        >
          Get Started
        </button>
      </div>
    </section>
  </template>
  
  <script setup>
  const scrollToStart = () => {
    const el = document.querySelector('#get-started');
    if (el) {
      el.scrollIntoView({ behavior: 'smooth' });
    }
  };
  </script>
  
  <style scoped>

  </style>
  