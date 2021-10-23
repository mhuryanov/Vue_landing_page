<script>
export default {
    data: () => {
        return {scale: document.body.clientWidth / 1440}
    },
    created() {
        window.addEventListener('resize', this.windowResizeHandler);
    },
    destroyed() {
        window.removeEventListener('resize', this.windowResizeHandler);
    },
    methods: {
        /**
         * Toggle menu
         */
        windowResizeHandler(e) {
            this.scale = document.body.clientWidth / 1440;
        },
    },
};
</script>
<style>
.section_home {
    width: 100%;
    position: relative;
}
/* (100vw / 1440px) * 800 */
.animation-hero-background {
    width: 2497px;
    height: 1800px;
    position: absolute;
    left: calc(60% - 1248.5px);
    top: calc(80% - 900px);
}
.bg-wrapper {
    position: inherit;
    width: 100%;
    height: calc((100vw / 1440) * 800);
    min-height: 260px;
    max-height: 100vh;
    background: black;
    overflow: hidden;
}
.hero-title {
    position: relative;
    z-index: 1;
}
.animation-hero-background img {
    --delay-time: 0.1;
    opacity: 0;
    position: absolute;
    transition: opacity 0.3s ease;
    -webkit-animation: fadeIn 0.5s forwards;
    animation: fadeIn 0.5s forwards;
}
.hero-bg-1 {
    left: 1040px;
    top: 0px;
}
.hero-bg-2 {
    left: 1472px;
    top: 449px;
}
.hero-bg-3 {
    left: 1775px;
    top: 779px;
    animation-delay: calc(var(--delay-time) * 13s) !important;
}
.hero-bg-5 {
    left: 680px;
    top: 633px;
    animation-delay: calc(var(--delay-time) * 13s) !important;
}
.hero-bg-6 {
    left: 928px;
    top: 148px;
}
.hero-bg-7 {
    left: 1908px;
    top: 458px;
    animation-delay: calc(var(--delay-time) * 14s) !important;
}
.hero-bg-9 {
    left: 914px;
    top: 920px;
    animation-delay: calc(var(--delay-time) * 15s) !important;
}
.hero-bg-10 {
    left: 468px;
    top: 1030px;
    animation-delay: calc(var(--delay-time) * 14s) !important;
}
.hero-bg-11 {
    left: 605px;
    top: 675px;
}
.hero-bg-12 {
    left: 281px;
    top: 814px;
}
.hero-bg-13 {
    left: 1700px;
    top: 429px;
}
.hero-bg-14 {
    left: 2424px;
    top: 723px;
}
.hero-bg-15 {
    left: 1172px;
    top: 30px;
    animation-delay: calc(var(--delay-time) * 15s) !important;
}
.hero-bg-16 {
    left: 1468px;
    top: 665px;
}
.hero-bg-17 {
    left: 0px;
    top: 680px;
    animation-delay: calc(var(--delay-time) * 12s) !important;
}
.hero-bg-18 {
    left: 1034px;
    top: 448px;
    animation-delay: calc(var(--delay-time) * 12s) !important;
}
.hero-bg-21 {
    left: 407px;
    top: 815px;
    animation-delay: calc(var(--delay-time) * 7s) !important;
}
.hero-bg-22 {
    left: 1230px;
    top: 244px;
    animation-delay: calc(var(--delay-time) * 8s) !important;
}
.hero-bg-24 {
    left: 310px;
    top: 30px;
}
.hero-bg-25 {
    left: 1102px;
    top: 633px;
    animation-delay: calc(var(--delay-time) * 2s) !important;
}
.hero-bg-26 {
    left: 1760px;
    top: 130px;
    animation-delay: calc(var(--delay-time) * 16s) !important;
}
.hero-bg-28 {
    left: 1698px;
    top: 486px;
    animation-delay: calc(var(--delay-time) * 5s) !important;
}
.hero-bg-29 {
    left: 613px;
    top: 449px;
    animation-delay: calc(var(--delay-time) * 9s) !important;
}
.hero-bg-30 {
    left: 2142px;
    top: 728px;
    animation-delay: calc(var(--delay-time) * 16s) !important;
}
.hero-bg-32 {
    left: 1540px;
    top: 632px;
    animation-delay: calc(var(--delay-time) * 11s) !important;
}
.hero-bg-34 {
    left: 610px;
    top: 148px;
    animation-delay: calc(var(--delay-time) * 17s) !important;
}
.hero-bg-36 {
    left: 840px;
    top: 468px;
    animation-delay: calc(var(--delay-time) * 6s) !important;
}
.hero-bg-38 {
    left: 2140px;
    top: 443px;
    animation-delay: calc(var(--delay-time) * 17s) !important;
}
.hero-bg-39 {
    left: 1472px;
    top: 152px;
    animation-delay: calc(var(--delay-time) * 3s) !important;
}
.hero-bg-40 {
    left: 370px;
    top: 244px;
    animation-delay: calc(var(--delay-time) * 1s) !important;
}
.hero-bg-41 {
    left: 875px;
    top: 740px;
    animation-delay: calc(var(--delay-time) * 4s) !important;
}
.hero-bg-43 {
    left: 1070px;
    top: 295px;
    animation-delay: calc(var(--delay-time) * 5s) !important;
}
.hero-bg-44 {
    left: 175px;
    top: 292px;
    animation-delay: calc(var(--delay-time) * 18s) !important;
}
.hero-bg-45 {
    left: 1998px;
    top: 268px;
    animation-delay: calc(var(--delay-time) * 17s) !important;
}
.hero-bg-46 {
    left: 1269px;
    top: 815px;
    animation-delay: calc(var(--delay-time) * 14s) !important;
}
@keyframes fadeIn {
    0% {
        opacity: 0;
    }
    100% {
        opacity: 1;
    }
}
</style>
<template>
    <section class="hero-1-bg" id="home">
        <div class="section_home">
            <div class="bg-wrapper">
                <div class="animation-hero-background" v-bind:style="'transform: scale(' + scale + ')'" >
                    <img src="../assets/images/hero-bg/hero-bg (1).png" class="hero-bg-1" />
                    <img src="../assets/images/hero-bg/hero-bg (2).png" class="hero-bg-2" />
                    <img src="../assets/images/hero-bg/hero-bg (3).png" class="hero-bg-3" />
                    <img src="../assets/images/hero-bg/hero-bg (5).png" class="hero-bg-5" />
                    <img src="../assets/images/hero-bg/hero-bg (6).png" class="hero-bg-6" />
                    <img src="../assets/images/hero-bg/hero-bg (7).png" class="hero-bg-7" />
                    <img src="../assets/images/hero-bg/hero-bg (9).png" class="hero-bg-9" />
                    <img src="../assets/images/hero-bg/hero-bg (10).png" class="hero-bg-10" />
                    <img src="../assets/images/hero-bg/hero-bg (11).png" class="hero-bg-11" />
                    <img src="../assets/images/hero-bg/hero-bg (12).png" class="hero-bg-12" />
                    <img src="../assets/images/hero-bg/hero-bg (13).png" class="hero-bg-13" />
                    <img src="../assets/images/hero-bg/hero-bg (14).png" class="hero-bg-14" />
                    <img src="../assets/images/hero-bg/hero-bg (15).png" class="hero-bg-15" />
                    <img src="../assets/images/hero-bg/hero-bg (16).png" class="hero-bg-16" />
                    <img src="../assets/images/hero-bg/hero-bg (17).png" class="hero-bg-17" />
                    <img src="../assets/images/hero-bg/hero-bg (18).png" class="hero-bg-18" />
                    <img src="../assets/images/hero-bg/hero-bg (21).png" class="hero-bg-21" />
                    <img src="../assets/images/hero-bg/hero-bg (22).png" class="hero-bg-22" />
                    <img src="../assets/images/hero-bg/hero-bg (24).png" class="hero-bg-24" />
                    <img src="../assets/images/hero-bg/hero-bg (25).png" class="hero-bg-25" />
                    <img src="../assets/images/hero-bg/hero-bg (26).png" class="hero-bg-26" />
                    <img src="../assets/images/hero-bg/hero-bg (28).png" class="hero-bg-28" />
                    <img src="../assets/images/hero-bg/hero-bg (29).png" class="hero-bg-29" />
                    <img src="../assets/images/hero-bg/hero-bg (30).png" class="hero-bg-30" />
                    <img src="../assets/images/hero-bg/hero-bg (32).png" class="hero-bg-32" />
                    <img src="../assets/images/hero-bg/hero-bg (34).png" class="hero-bg-34" />
                    <img src="../assets/images/hero-bg/hero-bg (36).png" class="hero-bg-36" />
                    <img src="../assets/images/hero-bg/hero-bg (38).png" class="hero-bg-38" />
                    <img src="../assets/images/hero-bg/hero-bg (39).png" class="hero-bg-39" />
                    <img src="../assets/images/hero-bg/hero-bg (40).png" class="hero-bg-40" />
                    <img src="../assets/images/hero-bg/hero-bg (41).png" class="hero-bg-41" />
                    <img src="../assets/images/hero-bg/hero-bg (43).png" class="hero-bg-43" />
                    <img src="../assets/images/hero-bg/hero-bg (44).png" class="hero-bg-44" />
                    <img src="../assets/images/hero-bg/hero-bg (45).png" class="hero-bg-45" />
                    <img src="../assets/images/hero-bg/hero-bg (46).png" class="hero-bg-46" />
                </div>
            </div>
            <div class="col-lg-12 text-center hero-title">
                <h1 class="hero-1-title font-weight-bold text-shadow mb-4">We create Next level <br />Experiences</h1>
            </div>
        </div>
    </section>
</template>
