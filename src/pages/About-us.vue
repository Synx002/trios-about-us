<template>
    <div class="scroll-section">
      <about-section-header-img />
      <about-section-markten />
      <about-section-team />
      <about-etc />
    </div>
  </template>
  
  <script>
  // eslint-disable-next-line vue/multi-word-component-names
  import AboutSectionHeaderImg from '../components/about-header-img.vue';
  import AboutSectionMarkten from '../components/about-section-markten.vue';
  import AboutSectionTeam from '../components/about-section-team.vue';
  import AboutEtc from '../components/about-etc.vue';
  
  export default {
    name: 'AboutUs',
    components: {
      AboutSectionHeaderImg,
      AboutSectionMarkten,
      AboutSectionTeam,
      AboutEtc,
    },
  };
  </script>
  
  <style scoped>
  .scroll-section{
    z-index: 1;
    background-color: var(--background-color--background-primary);
    min-height: 100vh;
    position: relative;
  }
  </style>
  