<template>
    <div class="row row-cols-1 row-cols-md-2  solutions_border">
        <div v-for="(item, i) in items" :key="item"
            :class="i === 0 || i === 1 || i === 9 || i === 8 ? `item-${i}` : 'solutions_items'"
            class="col-12 col-md-6 d-flex justify-content-start align-items-center">
            <img class="solutions_img"
                src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fitem.svg?alt=media&token=0446a22a-b096-424a-a9e7-16c8aae16f03"
                alt="items" />
            <p class="solutions_item">
                {{ item }}
            </p>
        </div>
    </div>
</template>

<script setup>

const items = ["Rango de precio dentro del cual se ubica el inmueble", "Qué tan atractivo es el inmueble en el mercado", "Valor de arriendo ideal", "Ventajas y desventajas del inmueble frente al sector", "Datos de valorización del sector", "Gastos notariales en caso de compra o venta", "Inmuebles similares para comparar o arrendar", "Comparativa por características del inmueble", "Datos catastrales del inmueble *", "Cómo se han comportado los precios en el sector"]

</script>

<style lang="scss" scoped>
.solutions_border {
    border: 1px solid #E9EBF1;
    border-radius: 16px;
}

.solutions_items {
    padding: 16px 20px;
    border: 1px solid #E9EBF1;
}

.item-0,
.item-1,
.item-8,
.item-9 {
    padding: 16px 20px;
    border: 1px solid #E9EBF1;
}

.item-0 {
    border-radius: 16px 0 0 0;
}

.item-1 {
    border-radius: 0 16px 0 0;
}

.item-8 {
    border-radius: 0 0 0 16px;
}

.item-9 {
    border-radius: 0 0 16px 0;
}

.solutions_item {
    font-weight: 600;
    font-size: 16px;
    letter-spacing: -0.01em;
    color: #282a33;
    margin: 0;
}

.solutions_img {
    width: 24px;
    margin: auto 10px;
}

@media (max-width: 992px) {
    .item-0 {
        border-radius: 16px 16px 0 0;
    }

    .item-1 {
        border-radius: 0 0 0 0;
    }

    .item-8 {
        border-radius: 0 0 0 0;
    }

    .item-9 {
        border-radius: 0 0 16px 16px;
    }
}
</style>