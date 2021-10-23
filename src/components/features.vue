<script>
import card from "./feature-card.vue";
import { LayoutIcon, LifeBuoyIcon, ServerIcon, RssIcon } from "vue-feather-icons";
export default {
  components: { LayoutIcon, LifeBuoyIcon, ServerIcon, RssIcon, card },
};
</script>
<style>
#features {
  background-color: #ddd9d9 !important;
}
.title-feature-header {
  font-family: MerriweatherUltraBold, AdobeInvisFont, MyriadPro-Regular;
  color: #303234;
  font-size: 36px;
}
.title-feature-header-2 {
  font-size: 25px;
  opacity: 0.8;
  font-family: Aller_Rg;
}
.card-content {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  max-width:1400px;
}
.button-group-1{
  padding-top:40px;
  display:flex;
  justify-content:center;
}
.feature-btn{
  margin-left:20px;
  height:81px;
  border-radius:20px;
  font-size:14px;
}
</style>
<template>
  <div>
    <!-- Features Start -->
    <section class="section bg-light feather-bg-img" id="features">
      <div class="container-fulid">
        <div class="row justify-content-center">
          <div class="col-lg-7">
            <div class="text-center mb-5">
              <h3 class="title-feature-header mb-3">You Name It. We’ll Produce It.</h3>
              <p class="title-feature-header-2">
                Whether your format is live, digital or hybrid, we’ll partner with you to
                produce experiences that engage the right audiences, increase brand
                awareness, build customer relationships and accelerate results.
              </p>
            </div>
          </div>
        </div>

        <div class="row align-items-center justify-content-center">
          <div class="col-lg-10 card-content">
            <card index="1" />
            <card index="2" />
            <card index="3" />
            <card index="4" />
            <card index="5" />
            <card index="6" />
          </div>
        </div>
      </div>
      <form action="#" class="row align-item-center button-group-1">
        <button type="submit" class="btn btn-primary feature-btn">LEARN MORE ABOUT OUR SERVICES</button>
        <button type="submit" class="btn btn-primary feature-btn">WATCH OUR REAL</button>
      </form>
    </section>
    <!-- Features End -->
  </div>
</template>
