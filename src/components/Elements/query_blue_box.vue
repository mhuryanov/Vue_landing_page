
<script>
export default {
    props:{
        index:String,
    }
};
</script>

<style>
.query-blue-box{
    width:318px;
    height:178px;
    border-radius:30px;
    background-color:#32B0CA;
    margin:10px;
    display:flex;
    justify-content:center;
    align-items: center;
}
.blue-box-inner{
    font-size:20px;
    opacity:0.8;
    color:white;
    font-family:Aller_Rg;
    padding:20px;
}
</style>

<template>
    <div class="query-blue-box">
        <div class="blue-box-inner" v-if="this.index=='1'">
            The majority of our client relationships last longer than 10 years.
        </div>
        <div class="blue-box-inner" v-if="this.index=='2'">
            Depending on the scope of the project, our turnaround time can be as fast as 4 weeks.
        </div>
        <div class="blue-box-inner" v-if="this.index=='3'">
            Our ratio of total registrations vs. attendance for digital events is 40% and 60% for live events. 
        </div>
        <div class="blue-box-inner" v-if="this.index=='4'">
            When asked how well an experience is organized, 96% of audiences respond “excellent.”
        </div>
    </div>
</template>