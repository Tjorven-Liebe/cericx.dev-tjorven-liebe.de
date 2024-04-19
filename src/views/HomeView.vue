<script setup>
import Navbar from "@/components/Navbar.vue";
import TopGraphic from "@/components/TopGraphic.vue";
import Features from '@/components/Features.vue'
</script>

<template>
  <main>
    <Navbar title="Tjorven-Liebe.de" :items=" { home: 'Home', features: 'Features', pricing: 'Pricing', faq: 'FAQ' } "/>
    <TopGraphic id="Home" image-source="https://tjorven-liebe.de/assets/web-developer-team.png" reference-links="[github: {link: 'https://github.com/tjorven-liebe', icon: 'github'}}"/>
    <Features/>
  </main>
</template>
