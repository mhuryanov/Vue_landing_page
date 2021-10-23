
<script>
export default {
    props:{
        index:String,
    }
};
</script>

<style>
.feature-box{
    width:315px;
    max-height:587px;
    border-radius:30px;
    background-color:white;
    margin:30px;
    box-shadow: 1px 10px 10px 1px rgba(0,0,0,.3);
}
.image-postion{
    text-align:center;
    margin-top:-30px;
}
.card-text-content{
    text-align:center;
    padding-top:20px;
    padding-bottom:40px;
}

.card-title{
    color:#303234;
    font-size:16px;
    font-family:Aller_Bd;
    margin-bottom:10px;
    height:60px;
    align-items: center;
    justify-content: center;
    display: flex;
}
.card-text{
    color:#303234;
    font-size:16px;
    font-family:Aller_Rg;
    line-height: 2.5;
}
</style>

<template>
    <div class="feature-box">
        <div v-if="this.index=='1'" class="image-postion">
            <img src="../assets/images/images/icon-live.png">
        </div>
        <div v-if="this.index=='2'" class="image-postion">
            <img src="../assets/images/images/icon-digital.png">
        </div>
        <div v-if="this.index=='3'" class="image-postion">
            <img src="../assets/images/images/icon-integrated-marketing.png">
        </div>
        <div v-if="this.index=='4'" class="image-postion">
            <img src="../assets/images/images/icon-tradeshows.png">
        </div>
        <div v-if="this.index=='5'" class="image-postion">
            <img src="../assets/images/images/icon-concact-center.png">
        </div>
        <div v-if="this.index=='6'" class="image-postion">
            <img src="../assets/images/images/icon-brand-activation.png">
        </div>
        <div v-if="this.index=='1'" class="card-text-content">
            <div class="card-title">LIVE</div>
            <a class="card-text">Conferences</a><br />
            <a class="card-text">Seminars</a><br />
            <a class="card-text">Product Launches</a><br />
            <a class="card-text">Business Dinners</a><br />
            <a class="card-text">Sporting Tournaments</a><br />
            <a class="card-text">Teambuilding</a><br />
            <a class="card-text">Employee</a><br />    
        </div>
        <div v-if="this.index=='2'" class="card-text-content">
            <div class="card-title">DIGITAL</div>
            <a class="card-text">Webinars</a><br />
            <a class="card-text">Virtual Conferences</a><br />
            <a class="card-text">Virtual Product Expos</a><br />
            <a class="card-text">Online Workshops</a><br />
            <a class="card-text">Online Entertainment</a><br />
            <a class="card-text">Virtual Teambuilding</a><br />
            <a class="card-text">Livestream</a><br />        
        </div>
        <div v-if="this.index=='3'" class="card-text-content">
            <div class="card-title">Integrated <br/>Marketing</div>
            <br />
            <a class="card-text">Design Services</a><br />
            <a class="card-text">Communications</a><br />
            <a class="card-text">CRM/ Email Marketing</a><br />
            <a class="card-text">Video Production</a><br />
            <a class="card-text">Social Media</a><br />    
        </div>
        <div v-if="this.index=='4'" class="card-text-content">
            <div class="card-title">Tradeshows</div>
            <a class="card-text">Sponsorships</a><br />
            <a class="card-text">Booth Production</a><br />
            <a class="card-text">Promotional Staffing</a><br />
            <a class="card-text">Lead Generation</a><br />
            <a class="card-text">Promotional Staffing</a><br />    
        </div>
        <div v-if="this.index=='5'" class="card-text-content">
            <div class="card-title">Contact  <br/>Center </div>
            <a class="card-text">Database Rental</a><br />
            <a class="card-text">Database Hygiene</a><br />
            <a class="card-text">Email Blasts</a><br />
            <a class="card-text">RSVP</a><br />
            <a class="card-text">Appointment Setting</a><br />
        </div>
        <div v-if="this.index=='6'" class="card-text-content">
            <div class="card-title">Brand  <br/>Activation</div>
            <a class="card-text">Curated Gift Kits</a><br />
            <a class="card-text">Sampling</a><br />
            <a class="card-text">Pop Ups</a><br />
            <a class="card-text">Installations</a><br />
            <a class="card-text">Swag</a><br />
        </div>
    </div>
</template>