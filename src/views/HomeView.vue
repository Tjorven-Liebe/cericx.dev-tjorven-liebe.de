<script setup>
import Navbar from "@/components/Navbar.vue";
import TopGraphic from "@/components/TopGraphic.vue";
import Features from '@/components/page/Features.vue'
import Pricing from '@/components/page/Pricing.vue'
</script>

<template>
  <main>
    <Navbar title="Tjorven-Liebe.de" :items=" { home: 'Home', features: 'Features', pricing: 'Pricing', faq: 'FAQ' } "/>
    <TopGraphic id="Home" image-source="https://tjorven-liebe.de/assets/web-developer-team.png"/>
    <Features/>
    <Pricing/>
  </main>
</template>
