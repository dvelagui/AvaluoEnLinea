<template>
    <div class="card">
            <img :src="cardImg" class="card-img-bottom position-relative" :alt="cardTitle" :style="cardTitle === 'Empresas' || cardTitle === 'Conexión API' ? 'margin-top: 17px' : ''">       
        <div class="card-body position-absolute">
            <h5 class="card-title">{{ cardTitle }}</h5>
            <p class="card-text">{{ cardText }}</p>
            <a :href="cardBtn" class="btn btn-primary">{{ cardBtnText }}</a>
        </div>
    </div>
</template>

<script setup>
import { toRefs, computed } from 'vue';


const props = defineProps({
    cardImg: String,
    cardTitle: String,
    cardText: String,
    cardBtn: String,
    cardBtnText: String,
});

const { cardImg, cardTitle, cardText, cardBtn, cardBtnText } = toRefs(props);


</script>

<style lang="scss" scoped>
.card {
    border: none;
    border-radius: none !important;
    padding: 0%;
    width: 25%;
}

.card-body {
    bottom: 0;
    background: linear-gradient(180deg, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.84) 71.31%);
}

.card-title {
    font-weight: 600;
    font-size: 32px;
    line-height: 100%;
    letter-spacing: -0.01em;
    color: #FFFFFF;
}

.card-text {
    font-weight: 400;
    font-size: 16px;
    line-height: 20px;
    letter-spacing: -0.01em;
    color: #FFFFFF;
}

.btn {
    font-family: 'Source Sans Pro';
    border-radius: 32px;
    font-weight: 600;
    font-size: 14px;
    line-height: 18px;
    text-align: center;
    letter-spacing: -0.01em;
    color: #FFFFFF;

}

@media (max-width: 992px) {
   .card {
    width: 100%;
    text-align: center;
   }
   .card-body {
    padding: 60px 32px;
}
}

</style>