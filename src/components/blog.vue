<script>
import { CalendarIcon, UserIcon } from "vue-feather-icons";
export default {
  components: {
    CalendarIcon,
    UserIcon
  }
};
</script>
<style>
#blog{
  background-color:#32B0CA !important;
}
.title-news{
  color:white;
  font-size:32px;
  font-family:Merriweather-Bold,AdobeInvisFont,MyriadPro-Regular;
  padding-top:32px;
}
.text-news{
  color:white;
  font-size:25px;
}
.news-back-size{
  width:98%;
  height:auto;
}
</style>

<template>
  <!-- Blog start -->
  <section class="section" id="blog">
    <div class="container-fulid">
      <div class="row justify-content-center">
        <div class="col-lg-6">
          <div class="text-center mb-5">
            <h3 class="title-news mb-3">We Work With The Best.</h3>
            <p
              class="text-news font-size-15"
            >For more than 20 years, we’ve been working with some of the most innovative clients on the Fortune 500.</p>
          </div>
        </div>
      </div>

      <div class="row">
        <img src="../assets/images/images/news-background.png" class="news-back-size">
      </div>
    </div>
  </section>
  <!-- Blog End -->
</template>