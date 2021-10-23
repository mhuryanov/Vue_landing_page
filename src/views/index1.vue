<script>
import Navbar from "@/components/navbar";
import Service from "@/components/services";
import Features from "@/components/features";
import Pricing from "@/components/pricing";
import Blog from "@/components/blog";
import Contact from "@/components/contact";
import Footer from "@/components/footer";

/**
 * Index-1
 */
export default {
  components: { Navbar, Service, Features, Pricing, Blog, Contact, Footer },
};
</script>
<style>
.section_home {
  display: flex;
  justify-content:center;
  color: white;
}
</style>
<template>
  <div>
    <Navbar />
    <div v-scroll-spy>
      <!-- Hero Start -->
      <section class="hero-1-bg" id="home"
                style="background-color: black; height: 701px"
      >
        <div
          class="container section_home"
        >
          <div class="row align-items-center justify-content-center">
            <div class="col-lg-12 text-center">
              <h1 class="hero-1-title font-weight-bold text-shadow mb-4">
                We create Next level <br />Experiences
              </h1>
            </div>
          </div>
        </div>
      </section>
      <!-- Hero End -->
      <Service />
      <Features />
      <Pricing />
      <Blog />
      <Contact />
      <Footer />
    </div>
  </div>
</template>
