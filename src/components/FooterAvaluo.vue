<template>
    <!-- Footer -->
    <div class="bg-footer text-white">
        <div class="container">
            <nav class="row">
                <a href="/" class="col-md-2 col-12 d-flex align-items-center justify-content-center my-3 mt-md-0">
                    <img src="src/assets/imgs/Logo-white.png" alt="Loogo Avaluo" class="img-logo">
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
                                <img src="src/assets/imgs/instagram.png" alt="Instagram">
                            </a>
                            <a class="nav-link px-2" href="#">
                                <img src="src/assets/imgs/twitter.png" alt="Twitter">
                            </a>
                            <a class="nav-link px-2" href="#">
                                <img src="src/assets/imgs/facebook.png" alt="Facebook">
                            </a>
                            <a class="nav-link px-2" href="#">
                                <img src="src/assets/imgs/linkedIn.png" alt="LinkedIn">
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