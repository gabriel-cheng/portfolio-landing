<script setup lang="ts">
import HeaderComponent from '@/components/HeaderComponent.vue';
import FooterComponent from '@/components/FooterComponent.vue';
import SectionOneComponent from '@/components/SectionOneComponent.vue';
import SectionTwoComponent from '@/components/SectionTwoComponent.vue';
import SectionThreeComponent from '@/components/SectionThreeComponent.vue';
</script>

<template>
  <HeaderComponent />
  <main id="main-container">
    <div class="main-subcontainer">
      <SectionOneComponent />
      <SectionTwoComponent />
      <SectionThreeComponent />
    </div>
  </main>
  <FooterComponent />
</template>

<style scoped>
#main-container {
  width: 100%;
  display: flex;
  justify-content: center;
  margin: 100px 0 0 0;
}
.main-subcontainer {
  max-width: 1800px;
  width: 100%;
}
</style>