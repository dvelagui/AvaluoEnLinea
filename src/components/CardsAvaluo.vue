<template>
    <div class="card">
        <img v-show="cardTitle === 'Empresas'" src='../assets/imgs/img_hero_inicio_empresas.png'
            class="card-img-top position-relative" :alt="cardTitle" :style="cardTitle === 'Empresas' ? '' : 'height: 0;'">
        <img v-show="cardTitle === 'Personas'" src='../assets/imgs/img_hero_inicio_personas.png'
            class="card-img-top position-relative" :alt="cardTitle"
            :style="cardTitle === 'Personas' ? '' : 'height: 0; visible: none'">
        <img v-show="cardTitle === 'Avalúo certificado'" src='../assets/imgs/img_hero_inicio_avaluo.png'
            class="card-img-top position-relative" :alt="cardTitle"
            :style="cardTitle === 'Avalúo certificado' ? '' : 'height: 0; visible: none'">
        <img v-show="cardTitle === 'Conexión API'" src='../assets/imgs/img_hero_inicio_API.png'
            class="card-img-top position-relative" :alt="cardTitle"
            :style="cardTitle === 'Conexión API' ? '' : 'height: 0; visible: none'">
        <div class="card-body  position-absolute">
            <h5 class="card-title">{{ cardTitle }}</h5>
            <p class="card-text">{{ cardText }}</p>
            <a :href="cardBtn" class="btn btn-primary">Ver más →</a>
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
});

const { cardImg, cardTitle, cardText, cardBtn } = toRefs(props);


const tpt = ["../assets/imgs/img_hero_inicio_empresas.png", "../assets/imgs/img_hero_inicio_empresas.png", "../assets/imgs/img_hero_inicio_empresas.png"
]

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