<script>
import {
  SendIcon,
  MailIcon,
  LinkIcon,
  PhoneCallIcon,
  ClockIcon,
  MapPinIcon,
} from "vue-feather-icons";
export default {
  components: {
    SendIcon,
    MailIcon,
    LinkIcon,
    PhoneCallIcon,
    ClockIcon,
    MapPinIcon,
  },
};
</script>

<style>
#contact {
  background-color: #604a4a !important;
}
.title-contact {
  color: white;
  font-size: 32px;
  font-family: Merriweather-Bold, AdobeInvisFont, MyriadPro-Regular;
}
.text-contact {
  color: white;
  opacity: 0.8;
  font-size: 25px;
}
.contact-input {
  text-align: center;
  width: 308px;
  height: 81px;
  border-radius: 15px;
  border: none;
  font-size: 18px;
  font-family: Aller_Bd;
  margin: 10px;
}
.contact-query-text {
  font-size: 20px;
  color: white;
  opacity: 0.8;
  font-family: Aller_Rg;
}
.form-check-label {
  font-size: 18px;
  color: white;
  padding-top: 3px;
  font-family: "Muli", sans-serif;
}
.form-check-input {
  border: none;
  border-radius: 10px;
  width: 24px;
  height: 24px;
  margin-right: 16px;
}
.form-check {
  width: 223px;
}
.contact-btn {
  width: 300px;
  height: 81px;
  border-radius: 16px;
}
</style>
<template>
  <!-- Contact Us Start -->
  <section class="section" id="contact">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-8">
          <div class="text-center mb-5">
            <h3 class="title-contact mb-3">Let’s Work Together.</h3>
            <p class="text-contact font-size-15">
              Whether you’re interested in our services or would like to be a member of
              our team, we’re happy to have a conversation. Tell us about your needs.
            </p>
          </div>
        </div>
      </div>
      <div class="row align-items-center     justify-content-center">
        <div class="row col-lg-12 justify-content-center">
          <input class="contact-input" placeholder="FIRST NAME" />
        </div>
        <div class="row col-lg-12 justify-content-center">
          <input class="contact-input" placeholder="LAST NAME" />
        </div>
        <div class="row col-lg-12 justify-content-center">
          <input class="contact-input" placeholder="WORK EMAIL" />
        </div>
        <div class="row col-lg-12 justify-content-center">
          <input class="contact-input" placeholder="PHONE NUMBERS" />
        </div>
        <div class="row col-lg-12 justify-content-center">
          <a class="contact-query-text">What best describes your needs?</a>
        </div>
        <div class="row col-lg-12 justify-content-center mt-5">
          <div class="form-check">
            <div class="row">
              <input type="checkbox" class="form-check-input" id="exampleCheck1" />
            </div>
            <label class="form-check-label" for="exampleCheck1">REQUEST OUR DECK</label>
          </div>
        </div>
        <div class="row col-lg-12 justify-content-center mt-3">
          <div class="form-check">
            <div class="row">
              <input type="checkbox" class="form-check-input" id="exampleCheck2" />
            </div>
            <label class="form-check-label" for="exampleCheck2">REQUEST A PROPOSAL</label>
          </div>
        </div>
        <div class="row col-lg-12 justify-content-center mt-3">
          <div class="form-check">
            <div class="row">
              <input type="checkbox" class="form-check-input" id="exampleCheck3" />
            </div>
            <label class="form-check-label" for="exampleCheck3"
              >INQUIRE ABOUT A JOB</label
            >
          </div>
        </div>
      </div>
      <form action="#" class="row align-item-center button-group-1">
        <button type="submit" class="btn btn-primary contact-btn">CONTACT US</button>
      </form>
      <div class="row col-lg-12 justify-content-center mt-5">
        <img src="../assets/images/images/Vector Smart Object@1X (2).png" />
      </div>
      <div class="row col-lg-12 justify-content-center mt-5 mb-5">
        <img src="../assets/images/images/facebook1@1X.png" class="mr-4"/>
        <img src="../assets/images/images/linkedin@1X.png" class="mr-4"/>
        <img src="../assets/images/images/email@1X.png" />
      </div>
    </div>
  </section>
  <!-- Contact Us End -->
</template>
