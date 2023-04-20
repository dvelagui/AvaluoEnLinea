<template>
    <div class="card" :style="FeaturesTitle === 'Precio justo e informado' ? 'border-left: 1px solid #E9EBF1; border-right: 1px solid #E9EBF1;' : ' '" >
        <img :src="FeaturesImg" class="card-img-top" :alt="FeaturesText">
        <div class="card-body">
            <h5 class="card-title">{{ FeaturesTitle }}</h5>
            <p class="card-text">{{ FeaturesText }} <a download href="#">{{ FeaturesUrl }}</a></p>
            <p class="card-text card-text2">{{ FeaturesText2 }}</p>
        </div>
    </div>
</template>

<script setup>
import { toRefs } from 'vue';


const props = defineProps({
    FeaturesImg: String,
    FeaturesTitle: String,
    FeaturesText: String,
    FeaturesUrl: String,
    FeaturesText2: String,
});

const { FeaturesImg, FeaturesTitle, FeaturesUrl, FeaturesText, FeaturesText2 } = toRefs(props)
</script>

<style lang="scss" scoped>
.card {
    width: 100%;
    max-width: 417px;
    padding: 40px 32px 10px 32px;    
    border-radius: none;
    border: none;
}

.card-img-top {
    width: 70px;
    text-align: center;
    margin: 0 auto;
}

h5 {
    font-weight: 600;
    font-size: 20px;
    line-height: 120%;
    text-align: center;
    letter-spacing: -0.01em;
    color: #282A33;
}

.card-text {
    font-weight: 400;
    font-size: 14px;
    line-height: 20px;
    text-align: center;
    letter-spacing: -0.01em;
    color: #6B7082;
}

.card-text2 {
    font-size: 12px;
}



@media (max-width: 992px) {}
</style>