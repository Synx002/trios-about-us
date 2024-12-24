<template>
  <div class="normal-nav" :class="{ 'hidden': isNavbarHidden }">
    <div class="navbar w-nav">
      <div class="navbar_container">
        <a href="" class="navbar_logo-link w-nav-brand">
          <div class="logo-nav w-embed">
            <img src="../assets/images/Logo.svg" alt="">
          </div>
        </a>
        <nav role="navigation" class="navbar_menu w-nav-menu">
          <div class="navbar_menu-links">
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Home
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Product Development
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Mechanical Engineering
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                About Trios
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Vacancies
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Contact
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <div class="locates-wrapper w-locales-list">
              <div class="dropdown w-dropdown" @click="toggleDropdown">
                <div class="locales-button w-dropdown-toggle">
                  <img src="../assets/images/Nederlands.svg" alt="" loading="lazy" class="locale-img">
                  <div class="nav-button-text w-icon-dropdown-toggle">
                    <img src="../assets/images/arrow-down.svg" alt="" loading="lazy">
                  </div>
                </div>
                <nav class="dropdown-list w-dropdown-list" :class="{ 'w-dropdown-list-open': isDropdownOpen }">
                  <div class="locale-list w-locales-items">
                    <div class="locale w-locale-items">
                      <img src="../assets/images/Nederlands.svg" alt="" class="locale-img">
                      <a href="" class="navbar_link language">Nederlands</a>
                    </div>
                    <div class="locale w-locale-items">
                      <img src="../assets/images/England.svg" alt="" class="locale-img">
                      <a href="" class="navbar_link language">England</a>
                    </div>
                  </div>
                </nav>
              </div>
            </div>
          </div>
        </nav>
      </div>
      <div class="w-nav-overlay"></div>
    </div>
  </div>
  
  <div class="sticky-nav" :class="{ 'visible': isStickyNavVisible }">
    <div class="sticky-navbar hide-tablet w-nav">
      <div class="navbar_container">
        <a href="" class="navbar_logo-link w-nav-brand">
          <div class="logo-nav w-embed">
            <img src="../assets/images/Logo.svg" alt="">
          </div>
        </a>
        <nav role="navigation" class="navbar_menu w-nav-menu">
          <div class="navbar_menu-links">
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Home
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Product Development
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Mechanical Engineering
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                About Trios
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Vacancies
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <a href="#" class="nav-button w-inline-block">
              <div class="nav-button-text">
                Contact
              </div>
              <div class="nav-button-overlay"></div>
            </a>
            <div class="locates-wrapper w-locales-list">
              <div class="dropdown w-dropdown" @click="toggleDropdown">
                <div class="locales-button w-dropdown-toggle">
                  <img src="../assets/images/Nederlands.svg" alt="" loading="lazy" class="locale-img">
                  <div class="nav-button-text w-icon-dropdown-toggle">
                    <img src="../assets/images/arrow-down.svg" alt="" loading="lazy">
                  </div>
                </div>
                <nav class="dropdown-list w-dropdown-list" :class="{ 'w-dropdown-list-open': isDropdownOpen }">
                  <div class="locale-list w-locales-items">
                    <div class="locale w-locale-items">
                      <img src="../assets/images/Nederlands.svg" alt="" class="locale-img">
                      <a href="" class="navbar_link language">Nederlands</a>
                    </div>
                    <div class="locale w-locale-items">
                      <img src="../assets/images/England.svg" alt="" class="locale-img">
                      <a href="" class="navbar_link language">England</a>
                    </div>
                  </div>
                </nav>
              </div>
            </div>
          </div>
        </nav>
      </div>
      <div class="corner-shape left-corner-top nav w-embed">
        <img src="../assets/images/download (13).svg" alt="">
      </div>
      <div class="corner-shape right-corner-top nav w-embed">
        <img src="../assets/images/download (12).svg" alt="">
      </div>
      <div class="w-nav-overlay"></div>
    </div>
    <div class="mobile-sticky-nav">
      <div id="mobile-menu" class="menu-nav_component">
        <div class="mobile-overlay-nav"></div>
        <div class="menu-nav_btn" @click="toggleMenu">
          <div class="menu-nav_icon-wrapper">
            <div class="menu-nav_icon is-open">
              <div class="menu-btn_icon-svg w-embed">
                <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M3 8H21" stroke="currentcolor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                <path d="M3 16H21" stroke="currentcolor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                </svg>
              </div>
            </div>
            <div class="menu-nav_icon is-close">
              <div class="menu-btn_icon-svg w-embed">
                <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M18 6L6 18" stroke="currentcolor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                <path d="M6 6L18 18" stroke="currentcolor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                </svg>
              </div>
            </div>
          </div>
        </div>
        <div id="mobile-menu" class="menu-nav_nav-links">
          <a href="" class="menu-nav_link-wrap w-inline-block">
            <div class="menu-nav_link">
              <div class="nav-button-text">Home</div>
            </div>
          </a>
          <a href="" class="menu-nav_link-wrap w-inline-block">
            <div class="menu-nav_link">
              <div class="nav-button-text">Product Development</div>
            </div>
          </a>
          <a href="" class="menu-nav_link-wrap w-inline-block">
            <div class="menu-nav_link">
              <div class="nav-button-text">Mechanical Engineering</div>
            </div>
          </a>
          <a href="" class="menu-nav_link-wrap w-inline-block">
            <div class="menu-nav_link">
              <div class="nav-button-text">About Trios</div>
            </div>
          </a>
          <a href="" class="menu-nav_link-wrap w-inline-block">
            <div class="menu-nav_link">
              <div class="nav-button-text">Vacancies</div>
            </div>
          </a>
          <a href="" class="menu-nav_link-wrap w-inline-block">
            <div class="menu-nav_link">
              <div class="nav-button-text">Contact</div>
            </div>
          </a>
          <div class="w-locales-list">
            <div class="location-mobile w-locales-items">
              <a href="#" class="location-link w-inline-block">
                <img src="../assets/images/Nederlands.svg" loading="lazy" alt="" class="locale-img is-mobile">
              </a>
            </div>
            <div class="location-mobile w-locales-items">
              <a href="#" class="location-link w-inline-block">
                <img src="../assets/images/England.svg" loading="lazy" alt="" class="locale-img is-mobile">
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import gsap from 'gsap';

export default {
  name: 'AppHeader',
  data() {
    return {
      isStickyNavVisible: window.innerWidth <= 768 ? true : false, // Sticky nav visible by default on mobile
      isDropdownOpen: false, // Dropdown status
      isMenuOpen: false,    // Menu status for toggling
    };
  },
  methods: {
    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen; // Toggle dropdown
    },

    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen; // Toggle menu status

      if (this.isMenuOpen) {
        gsap.to('.menu-nav_nav-links', { opacity: 1, display: 'block', duration: 0.3 });
        gsap.to('.menu-nav_icon.is-close', { display: 'block', duration: 0 });
        gsap.to('.menu-nav_icon.is-open', { display: 'none', duration: 0 });
        gsap.to('.mobile-overlay-nav', { opacity: 1, pointerEvents: 'auto', duration: 0.3 }); // Activate overlay
      } else {
        gsap.to('.menu-nav_nav-links', { opacity: 0, display: 'none', duration: 0.3 });
        gsap.to('.menu-nav_icon.is-close', { display: 'none', duration: 0 });
        gsap.to('.menu-nav_icon.is-open', { display: 'block', duration: 0 });
        gsap.to('.mobile-overlay-nav', { opacity: 0, pointerEvents: 'none', duration: 0.3 }); // Deactivate overlay
      }
    },


    handleScroll() {
      if (window.innerWidth <= 768) {
        this.isStickyNavVisible = true; // Sticky nav always visible on mobile
      } else {
        const scrollPosition = window.scrollY;

        if (scrollPosition > 200) {
          this.isStickyNavVisible = true;
        } else {
          this.isStickyNavVisible = false;
        }
      }

      this.isStickyNavVisible
        ? gsap.to('.sticky-nav', { opacity: 1, duration: 0.3 })
        : gsap.to('.sticky-nav', { opacity: 0, duration: 0.3 });
    },
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
    window.addEventListener('resize', this.handleScroll); // Recheck when resizing screen
  },
  beforeUnmount() {
    window.removeEventListener('scroll', this.handleScroll);
    window.removeEventListener('resize', this.handleScroll);
  },
};



</script>


<style scoped>
.normal-nav {
  width: 100%;
  height: 6rem;
  position: absolute;
}

.navbar {
  background-color: #ddd0;
  width: 100%;
  height: 100%;
  position: absolute;
  inset: 0% 0% auto;
}

.w-nav {
  z-index: 1000;
  position: relative;
}

.navbar_container {
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 100%;
  margin-left: auto;
  margin-right: auto;
  padding-left: 7%;
  padding-right: 7%;
  display: flex;
}

.w-nav-overlay {
  width: 100%;
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  right: 0;
  overflow: hidden;
}

.w-nav-brand {
  float: left;
  color: #333;
  text-decoration: none;
  position: relative;
}

.logo-nav {
  color: #fff;
  justify-content: center;
  align-items: center;
  display: flex;
}

.navbar_menu {
  align-items: center;
  display: block;
  position: static;
}

.w-nav-menu {
  float: right;
  position: relative;
}

.navbar_menu-links {
  grid-column-gap: .25rem;
  grid-row-gap: .25rem;
  justify-content: flex-start;
  align-items: center;
  display: flex;
}

.nav-button {
  background-color: var(--base-color-brand--white);
  text-align: center;
  border: 1px #000;
  border-radius: .5rem;
  padding: .6rem 1.25rem;
  text-decoration: none;
  position: relative;
}

.nav-button-text {
  z-index: 1;
  color: var(--base-color-brand--dark-blue);
  justify-content: center;
  align-items: center;
  margin-right: 0;
  font-size: 1rem;
  font-weight: 500;
  text-decoration: none;
  display: flex;
  position: relative;
}

.nav-button-overlay {
  z-index: 0;
  background-color: var(--base-color-brand--mid-blue);
  border-radius: .5rem;
  width: 100%;
  height: 100%;
  position: absolute;
  inset: auto 0% 0%;
}

.locales-button {
  display: flex; /* Mengatur elemen menjadi baris */
  align-items: center; /* Vertikal selaras tengah */
  gap: 8px; /* Memberi jarak antar elemen */
}

.locale-img {
  display: inline-block; /* Menjadikan gambar elemen inline */
}

.w-dropdown-toggle {
  -webkit-user-select: none;
  user-select: none;
  cursor: pointer;
  padding-right: 40px;
  display: inline-block;
}

.dropdown-list {
  background-color: #ddd0;
  border-radius: .4rem;
  box-shadow: 0 10px 20px #0000000f;
}

.w-dropdown-list {
  background: #ddd;
  min-width: 100%;
  display: none;
  position: absolute;
}

.w-dropdown-list {
  display: none;
}

.w-dropdown-list.w-dropdown-list-open {
  display: block;
}

.nav-button-overlay {
  z-index: 0;
  background-color: var(--base-color-brand--mid-blue);
  border-radius: .5rem;
  width: 100%;
  height: 0; 
  position: absolute;
  inset: auto 0% 0%;
  transform-origin: bottom; 
  transition: height 0.3s ease;
}

.navbar_menu-links .nav-button:hover .nav-button-overlay {
  height: 100%; 
}

.sticky-nav {
  z-index: 100;
  background-color: var(--base-color-brand--white);
  width: 100%;
  height: 4.1875rem;
  display: none;
  position: fixed;
  top: 0;
}

.sticky-navbar {
  background-color: var(--base-color-brand--white);
  width: 100%;
  height: 100%;
  position: absolute;
  inset: 0% 0% auto;
}

.navbar_container {
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 100%;
  margin-left: auto;
  margin-right: auto;
  padding-left: 7%;
  padding-right: 7%;
  display: flex;
}

.corner-shape.left-corner-top.nav {
  top: 3.8rem;
}

.corner-shape.left-corner-top {
  position: fixed;
  top: .75rem;
  left: .75rem;
}

.corner-shape.right-corner-top.nav {
  top: 3.8rem;
}

.corner-shape.right-corner-top {
  position: fixed;
  inset: .75rem .75rem auto auto;
}

.w-nav-overlay {
  width: 100%;
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  right: 0;
  overflow: hidden;
}

.w-nav-brand {
  float: left;
  color: #333;
  text-decoration: none;
  position: relative;
}

.navbar_menu {
  align-items: center;
  display: block;
  position: static;
}

.w-nav-menu {
  float: right;
  position: relative;
}

.navbar_menu-links {
  grid-column-gap: .25rem;
  grid-row-gap: .25rem;
  justify-content: flex-start;
  align-items: center;
  display: flex;
}

.sticky-nav-button {
  background-color: var(--base-color-brand--soft-blue);
  color: var(--background-color--background-tertiary);
  text-align: center;
  border: 1px #000;
  border-radius: .5rem;
  padding: .6rem 1.25rem;
  text-decoration: none;
  position: relative;
}

.sticky-nav-button-overlay {
  z-index: 0;
  background-color: var(--base-color-brand--mid-blue);
  border-radius: .5rem;
  width: 100%;
  height: 100%;
  position: absolute;
  inset: auto 0% 0%;
}

.w-inline-block {
  max-width: 100%;
  display: inline-block;
}

.w-dropdown {
  text-align: left;
  z-index: 900;
  margin-left: auto;
  margin-right: auto;
  display: inline-block;
  position: relative;
}

.locales-button {
  grid-column-gap: 8px;
  grid-row-gap: 8px;
  background-color: var(--base-color-brand--white);
  text-align: center;
  border: 1px #000;
  border-radius: .5rem;
  height: 2.6875rem;
  padding: .6rem 1.25rem;
  text-decoration: none;
  display: flex;
}

.w-dropdown-toggle {
  -webkit-user-select: none;
  user-select: none;
  cursor: pointer;
  padding-right: 40px;
  display: inline-block;
}


.w-icon-dropdown-toggle {
  width: 1em;
  height: 1em;
  margin: auto 20px auto auto;
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
}

.dropdown-list {
  background-color: #ddd0;
  border-radius: .4rem;
  box-shadow: 0 10px 20px #0000000f;
}

.w-dropdown-list {
  background: #ddd;
  min-width: 100%;
  display: none;
  position: absolute;
}

.mobile-sticky-nav {
    display: none;
}

.menu-nav_component {
    height: 4rem;
}

.menu-nav_btn {
  z-index: 1;
  grid-column-gap: 1rem;
  text-transform: uppercase;
  cursor: pointer;
  justify-content: space-between;
  align-items: center;
  padding: .5rem 2rem;
  display: flex;
  position: relative;
}

.menu-nav_icon-wrapper {
  width: 2rem;
  height: 2rem;
  position: relative;
}

.menu-nav_nav-links {
  z-index: 0;
  grid-row-gap: .5rem;
  transform-origin: 50% 0;
  background-color: #161616;
  flex-direction: column;
  justify-content: flex-start;
  align-items: stretch;
  margin-top: -1rem;
  padding: 1.5rem .5rem .5rem;
  display: flex;
  position: static;
  transform: translate(0);
}

.menu-nav_link-wrap {
  z-index: 2;
  position: relative;
  overflow: hidden;
}

.menu-nav_link {
  color: #fbf9fcb3;
  text-align: center;
  text-transform: capitalize;
  cursor: pointer;
  background-color: #232224;
  justify-content: center;
  padding: 1rem 2rem;
  display: flex;
  position: static;
}

.sticky-nav.visible {
  display: block;
  opacity: 1;
}

.locale-list {
  grid-column-gap: 16px;
  grid-row-gap: 16px;
  background-color: var(--base-color-brand--white);
  border-radius: .5rem;
  flex-flow: column;
  grid-template-rows: auto auto;
  grid-template-columns: 1fr 1fr;
  grid-auto-columns: 1fr;
  margin-top: .5rem;
  position: absolute;
  inset: 0% 0% auto auto;
  overflow: hidden;
}

.locale {
  grid-column-gap: 0rem;
  grid-row-gap: 0rem;
  background-color: var(--base-color-brand--white);
  flex-flow: row;
  grid-template-rows: auto auto;
  grid-template-columns: 1fr auto;
  grid-auto-columns: 1fr;
  justify-content: flex-start;
  align-items: center;
  padding: .2rem 1.8rem .2rem 1.25rem;
  display: flex;
}

img {
  width: auto;
  max-width: 100%;
  height: auto;
  display: inline-block;
}

.navbar_link.language {
  color: var(--base-color-brand--dark-blue);
  text-transform: none;
  font-size: 1rem;
  text-decoration: none;
}


.menu-nav_nav-links {
  display: none;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.menu-nav_nav-links.is-active {
  display: block;
  opacity: 1;
}

.menu-nav_icon.is-close {
  display: none;
}

.menu-nav_icon.is-open {
  display: block;
}
.menu-nav_icon-wrapper.is-active .is-close {
  display: none;
}
.menu-nav_icon-wrapper.is-active .is-open {
  display: block;
}

@media screen and (max-width: 991px) {
  .hide, .hide-tablet {
    display: none !important;
  }
  
  .mobile-sticky-nav {
    justify-content: flex-end;
    align-items: center;
    margin-top: 1rem;
    display: flex;
  }

  .logo-nav {
    z-index: 1;
    color: #fff;
    height: 100%;
    position: relative;
    display: flex;
  }

  .menu-nav_icon.is-close {
    inset: 0%;
  }
  .menu-nav_nav-links {
    background-color: var(--base-color-brand--white);
    border-radius: .5rem;
    justify-content: flex-start;
    align-items: stretch;
    margin-top: 0;
    margin-right: 2rem;
    padding-top: .5rem;
    position: relative;
  }
  .menu-nav_link-wrap {
    text-decoration: none;
  }

  .menu-nav_link {
    background-color: var(--base-color-brand--mid-blue);
    padding-top: .6rem;
    padding-bottom: .6rem;
  }

  .nav-button-text {
    text-decoration: none;
  }

  .location-mobile {
    grid-column-gap: 1rem;
    grid-row-gap: 1rem;
    justify-content: center;
    align-items: center;
    display: flex;
  }

  .location {
    justify-content: flex-start;
    align-items: center;
    width: 2rem;
    height: 100%;
    display: flex;
  }

  .locale-img.is-mobile {
    width: 2rem;  
  }

  #mobile-menu {
    display: flex;
    flex-direction: column; 
    gap: 10px; 
  }

  .menu-nav_link-wrap {
    display: block; 
    width: 100%;
    text-align: center;
  }

  .menu-nav_btn {
    color: var(--base-color-brand--dark-blue);
    background-color: #fff0;
    justify-content: flex-end;
    align-items: center;
    z-index: 999;
  }

  .menu-nav_icon-wrapper {
    background-color: var(--base-color-brand--dark-blue);
    text-align: center;
    border-radius: .5rem;
    width: 3rem;
    height: 3rem;
    inset: auto;
  }

  .menu-nav_icon {
    color: var(--base-color-brand--white);
    width: 3rem;
    height: 3rem;
  }

  .menu-btn_icon-svg {
    padding: 10px;
    align-items: center;
    display: flex;
    justify-content: center;
  }

  .mobile-overlay-nav {
    -webkit-backdrop-filter: blur(15px);
    backdrop-filter: blur(15px);
    pointer-events: none;
    background-color: #fff3;
    width: 100%;
    height: 100vh;
    position: absolute;
    inset: 0%;
    opacity: 0;
}
}

@media (max-width: 479px) {
  .sticky-navbar {
    padding-left: 1.5rem;
    padding-right: 1.5rem;
  }

  .logo-nav {
    z-index: 1;
    color: #fff;
    height: 100%;
    position: relative;
    display: flex;
  }

  .sticky-nav{
    background-color: transparent;
  }
  .navbar_menu{
    display: none;
  }

  .mobile-sticky-nav {
    display: block;
  }

  .menu-nav_nav-links {
    grid-row-gap: .3rem;
    margin-left: 1rem;
    margin-right: 1rem;
  }

  .nav-button-text, .button-text-46 {
    font-size: .875rem;
  } 

}
</style>
