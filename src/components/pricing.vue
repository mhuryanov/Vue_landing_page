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
.slide-react {
  width: 100%;
  height: 700px;
  background-repeat: round;
  display: flex;
  align-items: center;
  justify-content: space-around;
}
.slider {
  height: 420px;
}
.feedback-container {
  margin: 100px 100px 100px 100px;
  background-color: white;
  border-radius: 20px;
  box-shadow: 1px 10px 10px 1px rgba(0, 0, 0, 0.3);
}
.element-slider {
  text-align:center;
}
</style>
<script>
import queryBoxBlue from "./Elements/query_blue_box.vue";
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";
import Flickity from "vue-flickity";
import Slider from "vue-plain-slider";
export default {
  components: { queryBoxBlue, VueSlickCarousel, Flickity, Slider },
  data() {
    return {
      flickityOptions: {
        initialIndex: 3,
        prevNextButtons: true,
        pageDots: true,
        wrapAround: true,
        freeScroll: true,
        // any options from Flickity can be used
      },
    };
  },
  methods: {
    onSlideChangeStart(currentPage, el) {
      console.log("onSlideChangeStart", currentPage, el);
    },
    onSlideChangeEnd(currentPage, el) {
      console.log("onSlideChangeEnd", currentPage, el);
    },
  },
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
    <div
      :style="{
        'background-image':
          'url(' + require('@/assets/images/images/slider-bg.png') + ')',
      }"
      class="slide-react"
    >
      <Slider
        ref="Slider"
        direction="horizontal"
        :mousewheel-control="true"
        :performance-mode="true"
        :pagination-visible="true"
        :pagination-clickable="true"
        :loop="true"
        :speed="500"
        @slide-change-start="onSlideChangeStart"
        @slide-change-end="onSlideChangeEnd"
      >
        <div class="element-slider">
          <img src="@/assets/images/images/Shape 5 copy 2.png">
        </div>
        <div class="element-slider">
          <img src="@/assets/images/images/Shape 5 copy 2.png">
        </div>
        <div class="element-slider">
          <img src="@/assets/images/images/Shape 5 copy 2.png">
        </div>
        <div class="element-slider">
          <img src="@/assets/images/images/Shape 5 copy 2.png">
        </div>
      </Slider>
    </div>
  </section>

  <!-- Pricing End -->
</template>
