<template>
    <div>
        <div id="carouselExampleIndicators" class="carousel slide">
            <div class="carousel-indicators">
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"
                    aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
                    aria-label="Slide 2"></button>
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"
                    aria-label="Slide 3"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3"
                    aria-label="Slide 4"></button>
            </div>
            <div>
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <CardsAvaluo card-img="../assets/imgs/img_hero_inicio_personas.png" card-title="Empresas"
                            card-text="Ten herramientas para apoyar mejor tu proceso de ventas." card-btn="/empresas" />
                    </div>

                    <div class="carousel-item">
                        <CardsAvaluo card-img="../assets/imgs/img_hero_inicio_personas.png" card-title="Personas"
                            card-text="¿Quieres vender, comprar o arrendar una propiedad y tienes dudas sobre su valor?"
                            card-btn="/personas" />
                    </div>

                    <div class="carousel-item">
                        <CardsAvaluo card-img="../assets/imgs/img_hero_inicio_personas.png" card-title="Avalúo certificado"
                            card-text="Solicita un informe técnico firmado por un perito inscrito en el RAA."
                            card-btn="/avaluo-certificado" />
                    </div>

                    <div class="carousel-item">
                        <CardsAvaluo card-img="../assets/imgs/img_hero_inicio_personas.png" card-title="Conexión API"
                            card-text="Conecta la API a tus desarrollos y obtén todas las funcionalidades."
                            card-btn="/conexion-api" />
                    </div>


                </div>

            </div>
        </div>
        <!--   Hero Banner Cards Sections -->
    </div>
</template>

<script setup>

import CardsAvaluo from "./CardsAvaluo.vue";

</script>

<style lang="scss" scoped>
.carousel-indicators {
      bottom: 0;
    }
.carousel-indicators [data-bs-target] {
    width: 10px;
    height: 10px;
    border-radius: 50%;
}
    

</style>