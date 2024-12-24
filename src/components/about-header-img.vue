<template>
  <div class="section-header-img">
    <div class="gradient-logo"></div>
      <div class="header-img-overlay"></div>
        <img src="../assets/images/header-img.jpg" class="img-header">
      <div class="header-img-content">
        <div class="page-padding">
          <div class="img-header-title">
            <h1 class="heading-style-h1-big">
              <span class="red-text">Trios.</span>
              Reliable solutions for 30 years
            </h1>
          </div>
        </div>
      </div>
  </div>
  <div class="section-intro" style="background-color: #2b3467;">
    <div class="page-padding">
      <div class="spacer-xxhuge"></div>
      <div class="intro-text-grid">
        <div id="intro-wrapper" class="text-intro-wrapper">
          <div class="text-dot"></div>
          <p class="text-intro is-white">
            For 30 years, our team has treated every project as if it were our own, with a great sense of responsibility. About the result, about your budget and your secrets. We realize what your company really needs and ensure that the solution stands like a stone.
            <br>
            <br>
            We combine experience in various sectors and craftsmanship into customized solutions. In this, we go further than simply executing; we think along and always keep your interests in mind. That is where our strength lies. Trust in solutions that go beyond demand.
          </p>
        </div>        
      </div>
      <div class="spacer-xxhuge"></div>
    </div>
    <div class="divider-shape donw w-embed">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 78" fill="none" preserveAspectRatio="xMidYMid meet" style="display: block; line-height: 0;">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M407.949 0C401.35 0 396 5.34991 396 11.9494V32C396 38.6274 390.627 44 384 44H0V78H396H412H1440V0H407.949Z" fill="#ECF5FF"></path>
        </svg>
    </div>
  </div>
</template>
  
<script>
export default {
  name: 'AboutSectionHeaderImg', // Mengganti nama komponen menjadi multi-word
};
</script>
  
<style scoped>
.section-header-img{
  height: 100vh;
  position: relative;
}

.gradient-logo{
  z-index: 3;
  background-color: #c7919100;
  background-image: radial-gradient(circle farthest-side at 10% -10%, #fff, #fff0 46%);
  position: absolute;
  inset: 0%;
}

.header-img-overlay{
  cursor: none;
  mix-blend-mode: multiply;
  background-color: #2b346799;
  width: 100%;
  height: 100%;
  position: absolute;
  inset: 0%;
}

.img-header{
  object-fit: cover;
  width: 100%;
  height: 100%;
}

img{
  vertical-align: middle;
  width: auto;
  max-width: 100%;
  height: auto;
  display: inline-block;
}

.header-img-content{
  width: 100%;
  padding-bottom: 9.5rem;
  position: absolute;
  inset: auto 0% 0%;
}

.page-padding{
  margin-left: auto;
  margin-right: auto;
  padding-left: 7%;
  padding-right: 7%;
}

.img-header-title{
  width: 46.0625rem;
}

.heading-style-h1-big{
  color: #fff;
  font-size: 5rem;
}

h1 {
  color: var(--base-color-brand--dark-blue);
  margin-top: 0;
  margin-bottom: 0;
  font-family: Ppneuemontreal, Arial, sans-serif;
  font-size: 3.5rem;
  font-weight: 500;
  line-height: 110%;
}

.red-text{
  color: red;
}

.spacer-xxhuge {
  width: 100%;
  padding-top: 10rem;
}

.intro-text-grid {
  grid-column-gap: 1rem;
  grid-row-gap: 1rem;
  grid-template-rows: auto;
  grid-template-columns: 1.25fr 1.25fr 5.75rem;
  grid-auto-columns: 1fr;
  display: grid;
}

.text-intro-wrapper {
  display: flex;
  position: relative;
}

.text-dot {
  background-color: var(--base-color-brand--red);
  width: .375rem;
  height: .375rem;
  display: block;
  position: absolute;
  inset: .9rem auto 0% 0%;
}

.text-intro {
  text-indent: 1.5rem;
  font-size: 1.25rem;
}

.text-intro.is-white {
  color: var(--base-color-brand--white);
}

p {
  color: #7c7f8d;
  margin-bottom: 0;
  line-height: 170%;
}

.divider-shape.donw {
  bottom: -2px;
}

#intro-wrapper {
    grid-area: 1 / 2 / 2 / 3;
}

.divider-shape {
  width: 100%;
  display: block;
  position: relative;
}

.w-embed:before, .w-embed:after {
    content: " ";
    grid-area: 1 / 1 / 2 / 2;
    display: table;
}

.w-embed:after {
    clear: both;
}

@media (max-width: 1200px) {
  .heading-style-h1-big {
    font-size: 4rem;
  }

  .img-header-title {
    width: 35rem;
  }

  .intro-text-grid {
    grid-template-columns: 1fr 1fr;
  }

  .text-intro {
    font-size: 1.125rem;
  }
}

@media (max-width: 768px) {
  .heading-style-h1-big {
    font-size: 3rem;
  }

  .img-header-title {
    width: 100%;
  }

  .intro-text-grid {
    grid-template-columns: 1.25fr;
  }
  #intro-wrapper {
    grid-area: span 1 / span 1 / span 1 / span 1;
  }

  .text-intro {
    font-size: 1rem;
  }

  .spacer-xxhuge {
    padding-top: 5rem;
  }
  .page-padding {
    padding-left: 1rem;
    padding-right: 1rem;
  }
}

@media (max-width: 480px) {
  .heading-style-h1-big {
    font-size: 2.5rem;
  }

  .text-intro {
    font-size: 0.875rem;
    text-indent: 1rem;
  }

  .page-padding {
    padding-left: 5%;
    padding-right: 5%;
  }
}

</style>
  