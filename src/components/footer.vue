<script>
import {
  FacebookIcon,
  TwitterIcon,
  InstagramIcon,
  LinkedinIcon,
} from "vue-feather-icons";
export default {
  components: {
    FacebookIcon,
    TwitterIcon,
    InstagramIcon,
    LinkedinIcon,
  },
};
</script>

<style>
.footer-policy-title{
  font-size:16px;
  color:white;
  padding-right:5px;
}
.footer-row{
  align-items:center;
}
.footer-image{
  width:70%;
  height:auto;
  padding-left:5px;
}
.privacy-content{
  text-align: right;
}
.footer-main-image{
  width:70%;
}
</style>
<template>
  <div>
    <div class="footer-alt py-3">
      <div class="container-fulid">
        <div class="row footer-row">
          <div class="col-lg-2">
            <img src="../assets/images/images/Vector Smart Object.png" class="footer-image"/>
          </div>
          <div class="col-lg-8">
            <div class="text-center">
              <p class="text-white-50 font-size-15 mb-0">
                <img src="../assets/images/images/footer-title.png" class="footer-main-image"/>
              </p>
            </div>
          </div>
          <div class="col-lg-2 privacy-content">
            <a class="footer-policy-title">PRIVACY POLICY</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
