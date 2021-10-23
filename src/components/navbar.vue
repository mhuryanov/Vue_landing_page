<script>
import {
  FacebookIcon,
  TwitterIcon,
  InstagramIcon,
  LinkedinIcon,
  ArrowRightCircleIcon,
} from "vue-feather-icons";

export default {
  props: {
    navbarcolor: {
      type: Boolean,
      default: false,
    },
  },
  components: {
    FacebookIcon,
    TwitterIcon,
    InstagramIcon,
    LinkedinIcon,
    ArrowRightCircleIcon,
  },
    data: () => ({
    language:"english",
  }),
  mounted: () => {
    window.onscroll = function () {
      onwindowScroll();
    };
    var navbar = document.getElementById("navbar");
    function onwindowScroll() {
      if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
        navbar.classList.add("nav-sticky");
      } else {
        navbar.classList.remove("nav-sticky");
      }
    }
  },
  methods: {
    ToEnglish(){
      this.language="english";
    },
    ToSpanish(){
      this.language="spanish";
    },
        /**
     * Toggle menu
     */
    toggleMenu() {
      document.getElementById("navbarCollapse").classList.toggle("show");
    },
  },
};
</script>
<style>
.navbar-collapse {
  flex-grow: 0;
}
.nav-link {
  font-size: 13.46px !important;
  color: white !important;
}
.logo-dark {
  width: 49px;
  height: 44px;
}
.logo {
  display: flex;
  align-items: center;
}
.wrapper {
  width: 1400px;
  margin: 0 auto;
}
.fav-title {
  font-size: 35.91px;
  color: white;
  font-family: Aller_Rg;
  padding-left: 10px;
}
.back_query {
  background-color: #ed503e !important;
  border-radius: 10px;
  padding-right: 15px;
}
.navbar {
  display: block;
}
.switch-language {
  display: flex;
  justify-content: right !important;
  display:none;
}
.language-title{
  color: white;
  font-size: 12px;
  margin-right:15px;
  margin-left:15px;
  text-transform: uppercase;
  cursor: pointer;
}
.active-language{
  border-bottom:3px solid #32B0CA;
}
</style>
<template>
  <!--Navbar Start-->
  <nav
    class="navbar navbar-expand-lg fixed-top navbar-custom sticky sticky-dark"
    id="navbar"
    :class="{ 'navbar-light': navbarcolor === true }"
  >
    <div class="row container-fluid switch-language"><a class="language-title " @click="ToEnglish" :class="language == 'english' ? 'active-language' : ''">ENGLISH</a> | <a class="language-title" @click="ToSpanish" :class="language == 'spanish' ? 'active-language' : ''">Español</a></div>
    <div class="container-fluid">
      <!-- LOGO -->
      <a class="navbar-brand logo" href="/">
        <img src="@/assets/images/images/fav.png" alt class="logo-dark" />
        <span class="fav-title">Forums</span>
      </a>
      <button
        class="navbar-toggler"
        type="button"
        @click="toggleMenu()"
        aria-label="Toggle navigation"
      >
        <i class="mdi mdi-menu"></i>
      </button>
      <div class="collapse navbar-collapse" id="navbarCollapse">
        <ul class="navbar-nav mx-auto navbar-center" id="mySidenav" v-scroll-spy-active>
          <li class="nav-item">
            <a href="javascript: void(0);" v-scroll-to="{ el: '#services', offset: -1 }" class="nav-link"
              >WHO WE ARE</a
            >
          </li>
          <li class="nav-item">
            <a
              href="javascript: void(0);"
              v-scroll-to="{ el: '#features', offset: -2 }"
              class="nav-link"
              >WHAT WE DO</a
            >
          </li>
          <li class="nav-item">
            <a
              href="javascript: void(0);"
              v-scroll-to="{ el: '#pricing', offset: -3 }"
              class="nav-link"
              >HOW WE DO IT</a
            >
          </li>
          <li class="nav-item back_query">
            <a
              href="javascript: void(0);"
              v-scroll-to="{ el: '#contact', offset: -4 }"
              class="nav-link"
              >CONTACT US</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <!-- Navbar End -->
</template>
