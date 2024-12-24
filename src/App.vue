<template>
    <AppHeader />
    <main class="main-wrapper">
      <div class="dividers">
        <div class="divider top hide-tablet"></div>
        <div class="divider hide-tablet"></div>
      </div>
      <div class="page-section">
        <AboutUs />
        <app-footer />
      </div>
    </main>
</template>

<script>
import AppHeader from './components/app-header.vue';
import AppFooter from './components/app-footer.vue';
import AboutUs from './pages/About-us.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    AboutUs,
  },
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Raleway", sans-serif;
  font-weight: 400;
}

.app {
  min-height: 100vh;
  position: relative;
  background-color: #f1f1f1;
}
.container {
  padding: 0 20px;
  max-width: 1140px;
  margin: 0 auto;
}

.main-wrapper{
  background-color: #fff;
  border-radius: .5rem;
  flex-flow: column;
  margin: .75rem;
  display: flex;
}

.divider {
  z-index: 100;
  background-color: var(--base-color-brand--white);
  width: 100%;
  height: .75rem;
  position: fixed;
  inset: auto 0% 0%;
}
.page-sections {
    z-index: 1;
}

.divider.top {
    z-index: 100;
    inset: 0% 0% auto;
}

.divider {
    z-index: 100;
    background-color: var(--base-color-brand--white);
    width: 100%;
    height: .75rem;
    position: fixed;
    inset: auto 0% 0%;
}

@media screen and (max-width: 991px) {
    .hide, .hide-tablet {
        display: none !important;
    }
}
</style>