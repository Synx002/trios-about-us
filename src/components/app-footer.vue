<template>
  <div class="footer-section">
    <div class="page-padding">
      <div class="spacer-xxhuge"></div>
      <div class="footer-wrapper">
        <div class="footer-cta-wrapper">
          <h6 class="heading-style-h3">
            Ask us the impossible.
            <span class="red-text">Give us a problem</span>
            — we will find the solution!
          </h6>
          <div class="spacer-large">
            <a href="#" class="button w-inline-block">
              <div class="button-text">Get in touch</div>
              <div class="button-overlay" style="width: 100%; height: 0%;"></div>
            </a>
          </div>
        </div>
        <div class="footer-nav-items">
          <div class="footer-links">
            <a href="#" class="sticky-nav-button w-inline-block">
              <div class="nav-button-text">Home</div>
              <div class="sticky-nav-button-overlay" style="width: 100%; height: 0%;"></div>
            </a>
            <a href="#" class="sticky-nav-button w-inline-block">
              <div class="nav-button-text">Product Development</div>
              <div class="sticky-nav-button-overlay" style="width: 100%; height: 0%;"></div>
            </a>
            <a href="#" class="sticky-nav-button w-inline-block">
              <div class="nav-button-text">Mechanical Engineer</div>
              <div class="sticky-nav-button-overlay" style="width: 100%; height: 0%;"></div>
            </a>
            <a href="#" class="sticky-nav-button w-inline-block">
              <div class="nav-button-text">Vacancies</div>
              <div class="sticky-nav-button-overlay" style="width: 100%; height: 0%;"></div>
            </a>
            <a href="#" class="sticky-nav-button w-inline-block">
              <div class="nav-button-text">About Trios</div>
              <div class="sticky-nav-button-overlay" style="width: 100%; height: 0%;"></div>
            </a>
            <a href="#" class="sticky-nav-button w-inline-block">
              <div class="nav-button-text">Contact</div>
              <div class="sticky-nav-button-overlay" style="width: 100%; height: 0%;"></div>
            </a>
          </div>
        </div>
        <div class="footer-contact">
          <p class="text-size-medium dark">Contact</p>
          <div class="spacer-tiny"></div>
          <a href="#" class="footer-link">Nijverheidsweg 19 <br> NL-7161 AA Neede</a>
          <div class="spacer-small"></div>
          <a href="#" class="footer-link">+31 (0) 545 — 280 130</a>
          <a href="#" class="footer-link">info@trios.nl</a>
          <div class="spacer-small"></div>
          <div class="footer_social-list">
            <a href="" class="footer4_social-link">
              <img src="../assets/images/download (1).svg" alt="Facebook" class="social-icon" style="  fill: #ff0000;" />
            </a>
            <a href="" class="footer4_social-link">
              <img src="../assets/images/download.svg" alt="LinkedIn" class="social-icon" />
            </a>
          </div>
        </div>
      </div>
      <div class="spacer-xhuge hide-mobile-portrait"></div>
      <div class="divider-footer"></div>
      <div class="padding-top padding-medium">
        <div class="w-layout-grid footer_bottom-wrapper">
          <div class="footer_credit-text">© Trios</div>
          <a href="#" class="footer_legal-link">Privacy</a>
          <a href="#" class="footer_legal-link">General terms and conditions</a>
          <a href="#" class="footer_legal-link">Cookies</a>
        </div>
      </div>
      <div class="spacer-large"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AppFooter',
};
</script>

<style scoped>
.footer-section {
  background-color: var(--background-color--background-alternate);
  grid-template-rows: auto;
  grid-template-columns: 1fr 1fr 1fr;
  grid-auto-columns: 1fr;
  display: block;
  position: sticky;
  bottom: 0;
}

.page-padding {
  align-self: center;
  margin-left: auto;
  margin-right: auto;
  padding-left: 7%;
  padding-right: 7%;
}
.spacer-xxhuge {
  width: 100%;
  padding-top: 10rem;
}

.footer-wrapper{
  grid-column-gap: 16px;
  grid-row-gap: 16px;
  grid-template-rows: auto;
  grid-template-columns: 1fr 1fr 1fr;
  grid-auto-columns: 1fr;
  display: grid;
}

.spacer-xhuge {
  width: 100%;
  padding-top: 8rem;
}

.divider-footer {
  background-color: #7c7f8d33;
  height: 1px;
}

.padding-top {
  padding-right: 0rem !important;
  padding-bottom: 0rem !important;
  padding-left: 0rem !important;
}

.padding-medium {
  padding: 2rem;
}

.spacer-large {
  padding-top: 2.5rem;
}

.footer-cta-wrapper {
  width: 80%;
}

.heading-style-h3 {
  font-family: Ppneuemontreal, Arial, sans-serif;
  font-size: 2.5rem;
  font-weight: 500;
  line-height: 1.2;
}

h6 {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 1.25rem;
  font-weight: 500;
  line-height: 140%;
}

.button {
  z-index: 100;
  background-color: var(--base-color-brand--dark-blue);
  color: var(--base-color-brand--white);
  text-align: center;
  border-radius: .5rem;
  padding: .6rem 1.25rem;
  text-decoration: none;
  position: relative;
}

.w-inline-block {
  max-width: 100%;
  display: inline-block;
}

.button-text {
  z-index: 1;
  justify-content: flex-start;
  font-size: 1rem;
  font-weight: 500;
  display: flex;
  position: relative;
}

.button-overlay {
  background-color: #eb455f;
  border-radius: .5rem;
  width: 100%;
  height: 100%;
  position: absolute;
  inset: auto 0% 0%;
  overflow: hidden;
}

.footer-links {
  grid-column-gap: .25rem;
  grid-row-gap: .25rem;
  flex-flow: column;
  justify-content: flex-start;
  align-items: flex-start;
  display: flex;
}

.sticky-nav-button {
  background-color: #ecf5ff;
  color: #eb455f;
  text-align: center;
  border: 1px #000;
  border-radius: .5rem;
  padding: .6rem 1.25rem;
  text-decoration: none;
  position: relative;
}

.nav-button-text {
  z-index: 1;
  color: #2b3467;
  justify-content: center;
  align-items: center;
  margin-right: 0;
  font-size: 1rem;
  font-weight: 500;
  text-decoration: none;
  display: flex;
  position: relative;
}

.sticky-nav-button-overlay {
  z-index: 0;
  background-color: #dee7f4;
  border-radius: .5rem;
  width: 100%;
  height: 100%;
  position: absolute;
  inset: auto 0% 0%;
}

.footer-contact {
  flex-flow: column;
  display: flex;
}

.text-size-medium.dark {
  color: #2b3467;
}

.text-size-medium {
  font-size: 1.25rem;
  text-decoration: none;
}

p {
  color: #7c7f8d;
  margin-bottom: 0;
  line-height: 170%;
}

.spacer-tiny {
  width: 100%;
  padding-top: .125rem;
}

.footer-link {
  color: #7c7f8d;
  font-size: 1.25rem;
  line-height: 170%;
  text-decoration: none;
  transition: color .2s cubic-bezier(.86,0,.07,1);
}

.spacer-small {
  width: 100%;
  padding-top: 1rem;
}

.footer_social-list {
  white-space: normal;
  display: flex;
  flex-direction: flex-start;
  gap: 1rem;
}

.w-layout-grid {
  grid-row-gap: 16px;
  grid-column-gap: 16px;
  grid-template-rows: auto auto;
  grid-template-columns: 1fr 1fr;
  grid-auto-columns: 1fr;
  display: grid;
}

.footer4_social-link {
  justify-content: flex-start;
  align-items: center;
  text-decoration: none;
  display: flex;
}

.social-icon {
  width: 32px; 
  height: auto;
  transition: transform 0.3s ease;
}

.social-icon:hover {
  transform: scale(1.1);
}

svg:not(:root) {
  overflow: hidden;
}

svg:not(:root) {
  overflow-clip-margin: content-box;
  overflow: hidden;
}

.spacer-xhuge {
  width: 100%;
  padding-top: 8rem;
}

.divider-footer {
  background-color: #7c7f8d33;
  height: 1px;
}

.padding-top {
  padding-right: 0rem !important;
  padding-bottom: 0rem !important;
  padding-left: 0rem !important;
}

.padding-medium {
  padding: 2rem;
}

.footer_bottom-wrapper {
  grid-column-gap: 1.5rem;
  grid-row-gap: 0rem;
  white-space: normal;
  grid-template-rows: auto;
  grid-template-columns: max-content;
  grid-auto-columns: max-content;
  grid-auto-flow: column;
  justify-content: center;
  display: flex;
}

.spacer-large {
  padding-top: 2.5rem;
}

.spacer-large {
    padding-top: 2.5rem;
}

.footer_credit-text {
  color: #7c7f8d;
  font-size: .875rem;
}

.footer_legal-link {
  color: #7c7f8d;
  font-size: .875rem;
  text-decoration: none;
}

.red-text {
  color: #eb455f;
}

.w-embed:before, .w-embed:after {
  content: " ";
  grid-area: 1 / 1 / 2 / 2;
  display: table;
}

@media (max-width: 768px) {
  .hide-mobile-portrait{
    display: none;
  }

  .footer-wrapper {
    grid-template-columns: 1fr; /* Hanya satu kolom untuk ukuran layar kecil */
  }

  /* Menyembunyikan footer-cta-wrapper pada perangkat kecil */
  .footer-cta-wrapper {
    display: none;
  }

  .divider-footer{
    display: none;
  }

  .footer-contact {
    margin-top: 2rem;
  }
  
  /* Menyesuaikan padding dan font ukuran */
  .heading-style-h3 {
    font-size: 2rem;
  }

  .button {
    padding: .6rem 1rem;
    font-size: 0.875rem;
  }

  .social-icon {
    width: 28px;
    height: 28px;
  }

  .footer-links {
    flex-flow: wrap;
  }
  
  .page-padding{
    padding-left: 1rem;
    padding-right: 1rem;
  }

  .footer_bottom-wrapper{
    grid-column-gap: 2rem;
    grid-row-gap: .5rem;
    flex-flow: column;
    grid-auto-columns: max-content;
    place-items: stretch start;
    padding-bottom: 1rem;
    display: flex;
  }
}



</style>
