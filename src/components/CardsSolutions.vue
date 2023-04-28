<template>
    <div class="row d-flex justify-content-center">
        <div class="col-12 col-md-3 d-flex justify-content-start align-items-center shadow steps">
            <img :src="stepImg" :alt="stepText">
            <p>{{ stepText }}<span v-show="stepAst === 'true'"> *</span></p>
        </div>
    </div>
</template>

<script setup>
import { toRefs } from 'vue';


const props = defineProps({
    stepImg: String,
    stepText: String,
    stepAst: String
});

const { stepImg, stepText, stepAst } = toRefs(props);



const steps = [
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte_persona_01.png?alt=media&token=4bcb1f1e-ff66-4acf-9ce5-abf18d62c4ff',
        text: 'Determinar el valor de venta o renta de un inmueble',
        ast: false,
        report: 'personas'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte_persona_02.png?alt=media&token=5ce4f3ea-340f-428a-9392-5305c1ee3697',
        text: 'Dos inmuebles similares para comparar',
        ast: true,
        report: 'personas'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte_persona_03.png?alt=media&token=ec01959e-8d37-4849-9fac-42a0f968b10b',
        text: 'Qué tan atractivo es el inmueble en el mercado',
        ast: true,
        report: 'personas'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte_persona_04.png?alt=media&token=ec08a678-21f3-4b58-bf42-04e3ca67d1c9',
        text: 'Cómo se han comportado los precios en el sector',
        ast: true,
        report: 'personas'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte_persona_05.png?alt=media&token=d2d58f99-673b-4556-88ed-b14604291526',
        text: 'Comparativa por características del inmueble',
        ast: true,
        report: 'personas'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-0.png?alt=media&token=d93f1c33-1ff8-4b56-b8d8-9528dd48450c',
        text: 'Determinar el valor de venta o renta de un inmueble',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-1.png?alt=media&token=c9d84ef4-a0d7-48c6-b831-2522f5c91c18',
        text: 'Garantías bancarias',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-2.png?alt=media&token=050e7302-a471-4a05-abbf-615a699cb867',
        text: 'Trámites notariales',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-3.png?alt=media&token=1ad2bee4-39fc-4031-ad91-91a27c0a1f29',
        text: 'Reclamaciones ante catastro',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-4.png?alt=media&token=d9226a8c-4327-40ea-baa6-1cafc35d8b03',
        text: 'Aplicación de Normas Internacionales de Información Financiera',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-5.png?alt=media&token=b9b01a22-aeda-4a3c-a62f-6a8f7de79bcc',
        text: 'Cálculo de valores asegurables.',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-6.png?alt=media&token=56ac28fb-1332-4913-8535-57e78ffc1e9e',
        text: 'Procesos judiciales: Separación de bienes, restitución de bienes',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-7.png?alt=media&token=6b154245-1c3a-4b50-9a9d-0846b017fc29',
        text: 'Procesos judiciales: Procesos divisorios, sucesiones, remates',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FReporte-8.png?alt=media&token=f1ed503a-54ac-49a6-ae92-731952f5f3d5',
        text: 'Regularización de canon de arriendo, entre otros',
        ast: false,
        report: 'avaluo'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fapi_1.png?alt=media&token=867d428f-4c8d-42c7-b317-afc66e79d24e',
        text: 'Accesos a datos en tiempo real',
        ast: false,
        report: 'Api'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fapi_2.png?alt=media&token=8ef0ca66-9d54-4b27-949e-c2e77d627cf4',
        text: 'Ampliación de las funcionalidades',
        ast: false,
        report: 'Api'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fapi_3.png?alt=media&token=c8b07874-0bf7-4ee2-b5c5-ac2321c59db5',
        text: 'Integración con otros servicios',
        ast: false,
        report: 'Api'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fapi_4.png?alt=media&token=5dc0f3b9-d2de-4c71-a669-29648eec6f91',
        text: 'Mejora de la calidad de los datos',
        ast: false,
        report: 'Api'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fapi_5.png?alt=media&token=c4a5b4b2-70e2-448f-9098-b17f763f1701',
        text: 'Ahorro de tiempo y esfuerzo',
        ast: false,
        report: 'Api'
    },
    {
        img: 'https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fapi_6.png?alt=media&token=2f55c02f-6ee6-4548-8641-6fcd79ffc1c2',
        text: 'Reducción de los costos de desarrollo',
        ast: false,
        report: 'Api'
    },
]

</script>

<style lang="scss" scoped>
p {
    font-weight: 600;
    font-size: 16px;
    line-height: 120%;
    letter-spacing: -0.01em;
    color: #282A33;
    margin: 0;
}

span {
    color: #ca1d80;
}

.steps {
    width: 100%;
    max-width: 320px;
    padding: 24px;
    border-radius: 16px;
    margin: 16px;
}

.steps img {
    width: 72px;
    padding: 8px;
}
</style>