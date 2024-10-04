<!-- FeaturedArticlesSection.vue -->
<template>
    <section class="py-20 bg-gray-50">
      <div class="max-w-7xl mx-auto">
        <h2 class="text-3xl font-bold text-center mb-12">Featured Articles</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <article
            v-for="article in articles"
            :key="article.id"
            class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition"
          >
            <h3 class="text-2xl font-semibold mb-4">{{ article.title }}</h3>
            <p class="text-gray-600">{{ article.description }}</p>
            <a
              :href="article.link"
              class="block mt-6 text-indigo-500 font-bold hover:underline"
              >Read More</a
            >
          </article>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  const articles = [
    { id: 1, title: 'How to Start Competitive Programming', description: 'Get tips on starting your journey.', link: '#' },
    { id: 2, title: 'Top 10 Algorithms for Beginners', description: 'Learn essential algorithms every beginner should know.', link: '#' },
    { id: 3, title: 'Optimizing Code for Competitions', description: 'Improve your coding speed and efficiency.', link: '#' }
  ];
  </script>
  