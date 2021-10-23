<script>
import {
  FacebookIcon,
  TwitterIcon,
  InstagramIcon,
  LinkedinIcon,
  ArrowRightCircleIcon
} from "vue-feather-icons";

export default {
  props: {
    navbarcolor: {
      type: Boolean,
      default: false
    }
  },
  components: {
    FacebookIcon,
    TwitterIcon,
    InstagramIcon,
    LinkedinIcon,
    ArrowRightCircleIcon
  },
  mounted: () => {
    window.onscroll = function() {
      onwindowScroll();
    };
    var navbar = document.getElementById("navbar");
    function onwindowScroll() {
      if (
        document.body.scrollTop > 50 ||
        document.documentElement.scrollTop > 50
      ) {
        navbar.classList.add("nav-sticky");
      } else {
        navbar.classList.remove("nav-sticky");
      }
    }
  },
  methods: {
    /**
     * Toggle menu
     */
    toggleMenu() {
      document.getElementById("navbarCollapse").classList.toggle("show");
    }
  }
};
</script>
<style>
.navbar-collapse{
  flex-grow:0;
}
.nav-link
{
  font-size:16px !important;
  color:white !important;
}
.back_query{
}
.logo-dark{
  width:224px;
  height:54px;
}
.wrapper{
    width: 1400px;
    margin: 0 auto;
}
@media (min-width: 1200px)
<style>
.container, .container-sm, .container-md, .container-lg, .container-xl {
    max-width: 1400px !important;
}
</style>
<template>
  <!--Navbar Start-->
  <nav
    class="navbar navbar-expand-lg fixed-top navbar-custom sticky sticky-dark"
    id="navbar"
    :class="{'navbar-light': navbarcolor === true}"
  >
    <div class="container-fluid">
      <!-- LOGO -->
      <a class="navbar-brand logo" href="/">
        <img src="@/assets/images/images/Vector Smart Object.png" alt class="logo-dark" height="24" />
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
            <a href="javascript: void(0);" v-scroll-to="'#services'" class="nav-link">WHO WE ARE</a>
          </li>
          <li class="nav-item">
            <a
              href="javascript: void(0);"
              v-scroll-to="{ el: '#features', offset: -2}"
              class="nav-link"
            >WHAT WE DO</a>
          </li>
          <li class="nav-item">
            <a
              href="javascript: void(0);"
              v-scroll-to="{ el:'#pricing', offset: -2}"
              class="nav-link"
            >HOW WE DO IT</a>
          </li>
          <li class="nav-item">
            <a
              href="javascript: void(0);"
              v-scroll-to="{ el:'#contact', offset:-50}"
              class="nav-link back_query"
            >CONTACT US</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <!-- Navbar End -->
</template>

