<!-- HomeView.vue -->
<template>
  <div>
    <Header />
    <main class="pt-16">
      <HeroSection />
      <FeaturedArticlesSection />
      <LinkToRoadmapSection />
    </main>
  </div>
</template>

<script setup>
import AppHeader from "@/components/AppHeader.vue";
import HeroSection from '@/components/HeroSection.vue';
import FeaturedArticlesSection from '@/components/FeaturedArticlesSection.vue';
import LinkToRoadmapSection from '@/components/LinkToRoadmapSection.vue';
</script>
