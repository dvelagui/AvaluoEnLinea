<template>
    <div class="position-relative d-flex flex-column justify-content-center align-items-center hero-banner">
        <img class="hero-banner_img" :src="imgBanner" :alt="titleBanner">
        <img class="hero-banner_img_mobile" :src="imgBannerMobile" :alt="titleBanner">
        <div class="position-absolute text-center hero-banner_content">
            <h2 class="hero-banner_title">{{ titleBanner }}</h2>
            <h2 class="hero-banner_subtitle">{{ subtitleBanner }}</h2>
            <div class="row d-flex flex-row justify-content-center align-items-center mt-5">              
                    <a class="col-4 col-md-2 mx-2 btn btn-primary" :class="btnBanner2 ? 'col-md-2' : 'col-md-4'" href="#Solutions">{{ btnBanner1 }}</a>     
                    <a class="col-4 col-md-2 mx-2 btn hero-banner_btn2" :style="btnBanner2 ? ' ' : 'display:none'" href="#Pricing">{{ btnBanner2 }}</a>              
            </div>
        </div>
    </div>

</template>

<script setup>
import { toRefs } from 'vue';


const props = defineProps({
    titleBanner: String,
    subtitleBanner: String,
    btnBanner1: String,
    btnBanner2: String,
    imgBanner: String,
    imgBannerMobile: String,
});

const { titleBanner, subtitleBanner, btnBanner1, btnBanner2, imgBanner } = toRefs(props);


</script>

<style lang="scss" scoped>

.hero-banner_content {
    bottom: 10%;
}
.hero-banner_title {
    font-family: 'Comfortaa';
    font-weight: 700;
    font-size: 42px;
    line-height: 100%;
    letter-spacing: -0.01em;
    color: #FFFFFF;
}

.hero-banner_subtitle {
    font-family: 'Comfortaa';
    font-weight: 700;
    font-size: 20px;
    line-height: 120%;
    letter-spacing: -0.01em;
    color: #FFFFFF;
    margin-top: 12px;
}


.btn {
    font-family: 'Source Sans Pro';
    border-radius: 32px;
    font-weight: 600;
    font-size: 16px;
    line-height: 18px;
    text-align: center;
    letter-spacing: -0.01em;
    padding: 14px 24px;
}


.hero-banner_btn2 {
    background-color: #FFFFFF;
    color: #282A33;
}
.hero-banner_btn2:hover {
    background-color: #FFFFFF;
}

.hero-banner_img {
    z-index: -99;
}
.hero-banner_img_mobile {
    z-index: -99;
    display: none;
}

@media (max-width: 992px) {
    .hero-banner_img {
    display: none;
    }
    .hero-banner_img_mobile {
    display: block;
    width: 100%;
}
}
</style>