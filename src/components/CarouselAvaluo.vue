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
                        <CardsAvaluo
        card-img="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fimg_hero_inicio_empresas.png?alt=media&token=7debb63b-1708-42e9-8596-750add0e01b7"
        card-title="Empresas"
        card-text="Ten herramientas para apoyar mejor tu proceso de ventas."
        card-btn="/empresas"
        card-btn-text="Ver más →"
      />
                    </div>

                    <div class="carousel-item">
                        <CardsAvaluo
        card-img="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fimg_hero_inicio_personas.png?alt=media&token=7e749742-8b7c-45fd-8698-8750ae18e163"
        card-title="Personas"
        card-text="¿Quieres vender, comprar o arrendar una propiedad y tienes dudas sobre su valor?"
        card-btn="/personas"
        card-btn-text="Haz tu avalúo →"
      />
                    </div>

                    <div class="carousel-item">
                        <CardsAvaluo
        card-img="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fimg_hero_inicio_avaluo.png?alt=media&token=e08e26d4-0aa8-465b-ad72-983f659d51cf"
        card-title="Avalúo Certificado"
        card-text="Solicita un informe técnico firmado por un perito inscrito en el RAA."
        card-btn="/avaluo-certificado"
        card-btn-text="Conoce más →"
      />
                    </div>

                    <div class="carousel-item">
                        <CardsAvaluo
        card-img="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fimg_hero_inicio_API.png?alt=media&token=653296ff-7a48-438c-8f9b-4ff8b37cb1d5"
        card-title="Conexión API"
        card-text="Conecta la API a tus desarrollos y obtén todas las funcionalidades."
        card-btn="/conexion-api"
        card-btn-text="Ingresar →"
      />
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