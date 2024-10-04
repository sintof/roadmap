<!-- Header.vue -->
<template>
    <header class="fixed top-0 left-0 w-full bg-gray-800 backdrop-blur-lg shadow-md p-4 z-50">
      <nav class="flex justify-between items-center max-w-7xl mx-auto">
        <div class="text-2xl font-bold text-white">CompProgPrep</div>
        <ul class="flex space-x-6">
          <li v-for="link in links" :key="link.name">
            <a
              :href="link.url"
              class="text-white text-lg transition duration-300 ease-in-out hover:text-indigo-400"
              >{{ link.name }}</a
            >
          </li>
        </ul>
      </nav>
    </header>
  </template>
  
  <script setup>
  const links = [
    { name: 'Home', url: '#' },
    { name: 'Get Started', url: '#get-started' },
    { name: 'Roadmap', url: '#roadmap' },
    { name: 'Articles', url: '#articles' },
    { name: 'About Us', url: '#about-us' }
  ];
  </script>
  
  <style scoped>
  header {
    backdrop-filter: blur(10px);
    box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.1);
  }
  </style>
  