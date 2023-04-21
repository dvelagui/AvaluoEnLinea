<template>
    <!-- Footer -->
    <div class="bg-footer text-white">
        <div class="container">
            <nav class="row">
                <a href="/" class="col-md-2 col-12 d-flex align-items-center justify-content-center my-3 mt-md-0">
                    <img src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FLogo-white.png?alt=media&token=c9b9643d-4c31-4260-9ecd-ab9072cae3ca" alt="Loogo Avaluo" class="img-logo">
                </a>
                <ul class="col-md-2 col-6 list-unstyled d-flex flex-column  p-md-4 px-4 py-2 mb-0">
                    <li class="nav-item">
                        <a class="nav-link" href="/empresas" aria-current="page">Empresas</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="/personas">Personas</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#form-contact">Contacto</a>
                    </li>
                </ul>
                <ul class="col-md-2 col-6  list-unstyled d-flex flex-column p-md-4 px-4 py-2 mb-0">
                    <li class="nav-item">
                        <a class="nav-link" href="/avaluo-certificado" aria-current="page">Avalúo Certificado</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="/conexion-api">Conexión API</a>
                    </li>
                </ul>
                <ul class="col-md-3 col-12 list-unstyled d-flex flex-column p-md-4 px-4 py-2 mb-0">
                    <li class="nav-link">
                        Horario de Atención
                    </li>
                    <p class="open-hours">Lunes - Viernes 8:00 am - 8:00 pm</p>
                    <p class="open-hours">Sábados 8:00 am - 2:00 pm</p>
                    <li class="nav-item">
                        <a class="nav-link" href="#">WhatsApp</a>
                    </li>
                </ul>
                <div class="col-md-3 col-12 list-unstyled d-flex flex-column justify-content-between align-items-start  p-md-4 px-4 py-2">
                    <ul class="list-unstyled d-flex justify-content-start">
                        <li class="nav-link">
                            Síguenos:
                        </li>
                        <li class="nav-item ml-2 d-flex justify-content-start">
                            <a class="nav-link px-2" href="#">
                                <img src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Finstagram.png?alt=media&token=05398746-f2cf-4de5-ada9-cbc484e6bb0a" alt="Instagram">
                            </a>
                            <a class="nav-link px-2" href="#">
                                <img src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Ftwitter.png?alt=media&token=d75a355c-8dc2-4458-bd48-99394501f0b4" alt="Twitter">
                            </a>
                            <a class="nav-link px-2" href="#">
                                <img src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Ffacebook.png?alt=media&token=c7c32c5d-c640-47f6-ae4d-e4a82e2d3d3c" alt="Facebook">
                            </a>
                            <a class="nav-link px-2" href="#">
                                <img src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FlinkedIn.png?alt=media&token=898a7035-294f-4a53-8836-6d421416df5d" alt="LinkedIn">
                            </a>
                        </li>
                    </ul>
                    <p class="copyRight">Avalúo en línea. Todos los derechos reservados. © 2023.</p>
                </div>
            </nav>
        </div>

    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>

.bg-footer {
    background-color: #282A33;
}
.nav-link {
    font-weight: 600;
    font-size: 14px;
    line-height: 18px;
    color: white;
    padding: 6px 0;
}

.open-hours {
    font-weight: 400;
    font-size: 14px;
    line-height: 18px;
    color: white;
    padding: 0;
    margin: 0;
}

.copyRight {
    font-weight: 400;
    font-size: 12px;
    line-height: 120%;
    text-align: center;
    letter-spacing: -0.01em;
}

@media (max-width: 992px) {
    .copyRight {
   background-color: #16171D;
    text-align: center;
    width: 100%;
    padding: 10px;
}

}
</style>