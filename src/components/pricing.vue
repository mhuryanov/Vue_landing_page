<style>
.title-pricing {
  font-size: 36px;
  font-family: MerriweatherUltraBold, AdobeInvisFont, MyriadPro-Regular;
}
.text-pricing {
  font-size: 25px;
}
.bt-image-size-pricing {
  width: 100%;
  height: auto;
}
</style>
<script>
import queryBoxBlue from "./Elements/query_blue_box.vue";
  import VueSlickCarousel from 'vue-slick-carousel'
    import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
export default {
  components: { queryBoxBlue,VueSlickCarousel  },
};
</script>
<template>
  <!-- Pricing Start -->
  <section class="section bg-light" id="pricing">
    <div class="container-fulid">
      <div class="row justify-content-center">
        <div class="col-lg-8">
          <div class="text-center mb-5">
            <h3 class="title-pricing mb-3">
              It’s Not Just What We Do.<br />
              It’s How We Do It.
            </h3>
            <p class="text-pricing font-size-15">
              Great customer service requires a deep understanding of your needs, goals
              and expectations. We’ve developed a personalized planning process that
              aligns itself to yours- from creating the concept to analyzing the results.
            </p>
          </div>
        </div>
      </div>
      <div class="row">
        <img
          src="../assets/images/images/display_complexing.png"
          class="bt-image-size-pricing"
        />
      </div>
      <div class="text-center mb-5 mt-5">
        <h3 class="title-pricing mb-3">By The Numbers:</h3>
      </div>
      <div class="row justify-content-center mb-5">
        <queryBoxBlue index="1" />
        <queryBoxBlue index="2" />
        <queryBoxBlue index="3" />
        <queryBoxBlue index="4" />
      </div>
      <div class="row justify-content-center">
        <div class="col-lg-7">
          <div class="text-center mb-5">
            <h3 class="title-pricing mb-3">We Love Our Clients.</h3>
            <p class="text-pricing font-size-15">
              Keeping our clients happy is at the heart of everything we do. That’s why
              we’re proud to have built long-lasting relationships with most of them.
              <strong>Here’s what they have to say about us:</strong>
            </p>
          </div>
        </div>
      </div>
    </div>
                    <div class="container">
                    <div class="ts-title">
                        <h2>Testimonials</h2>
                    </div>
                    <!--end ts-title-->
                    <div class="row">
                        <div class="col-md-8 offset-md-2">
                            <div class="owl-carousel" data-owl-dots="1" data-owl-loop="1" data-animate="ts-fadeInUp">
                                <div class="slide mb-5">
                                    <p class="ts-h5">
                                        In id nulla magna. Nullam posuere fermentum mattis. Nunc id dui at sapien faucibus
                                        fermentum ut vel diam. Nullam tempus, nunc id efficitur sagittis
                                    </p>
                                    <div class="ts-circle__lg mb-3" data-bg-image="assets/img/person.jpg"></div>
                                    <h5>Jane Doe</h5>
                                    <h6 class="ts-opacity__40">Bristol Creative</h6>
                                </div>
                                <!--end slide-->
                                <div class="slide mb-5">
                                    <p class="ts-h5">
                                        Nam egestas porta posuere. Nunc velit lorem, vestibulum vitae massa nec, lacinia dictum
                                        ligula. Quisque scelerisque nec dolor id convallis. Vestibulum porta ipsum pretium
                                        turpis rhoncus, non fringilla ipsum mattis.
                                    </p>
                                    <div class="ts-circle__lg mb-3" data-bg-image="assets/img/person-02.jpg"></div>
                                    <h5>John Brown</h5>
                                    <h6 class="ts-opacity__40">ABC Architects</h6>
                                </div>
                                <!--end slide-->
                            </div>
                            <!--end owl-carousel-->
                        </div>
                        <!--end col-md-8-->
                    </div>
                    <!--end row-->
                </div>
  </section>
  
  <!-- Pricing End -->
</template>
