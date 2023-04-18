<template>
    <nav class="navbar navbar-expand-lg mt-5">
        <div class="container a-box-shadow">
            <a href="/">
                <img alt="Logo Avaluo" class="logo" src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Favaluo_logo.png?alt=media&token=1723c063-cf47-4ef2-8c0a-0eac7b4eb74e" />
            </a>
            <button  class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="true" aria-label="Toggle navigation">
            <span class="menu-mobile">Menú</span>
                <span class="navbar-toggler-icon" style="background-image: url('data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%2833, 37, 41, 0.75%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e')" @click="openMenu(true)" v-if="!isMenuOpen" ></span>
                <span class="navbar-toggler-icon" style="background-image: url('https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Fclose.svg?alt=media&token=7b605e05-c2c9-47a4-81ca-e02e2b915302')" @click="openMenu(false)" v-else></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                    <li class="nav-item" v-for="link in links" :key="link.name">
                        <a class="nav-link" :href="link.href">{{ link.name }}<img :id="link.name" :class="titlePage == link.name ? 'selection active' : 'selection'" src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2FChevron.png?alt=media&token=317592c7-04d9-4b96-a225-c07733a05132"
                                alt="Selection" width="15" ></a>
                    </li>
                </ul>
                <a  @click="btnAccess()" class="nav-btn-access">Ingresar</a>
            </div>
        </div>
    </nav>
</template>

<script setup>
import { ref } from "vue";
import { toRefs } from 'vue';

const props = defineProps({
    titlePage: String
});

const { titlePage } = toRefs(props);

const isMenuOpen = ref(false);

const openMenu = (action) => {
  isMenuOpen.value = action;
}

const btnAccess = () => {
    alert("QUieres Ingresar???")
}


const links = [
    {
        name: "Inicio",
        href: "/"
    },
    {
        name: "Empresas",
        href: "/empresas"
    },
    {
        name: "Personas",
        href: "/personas"
    },
    {
        name: "Avalúo Certificado",
        href: "/avaluo-certificado"
    },
    {
        name: "Conexión API",
        href: "/conexion-api"
    },
]


</script>


<style lang="scss" scoped>
.logo {
    width: 116px;
}

.a-box-shadow {
    background: #FFFFFF;
    box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.05);
}

.navbar>.container {
    justify-content: space-around;

}

.navbar-toggler {
    border: none;
    border-radius: none;
}

.navbar-toggler:focus {
    box-shadow:  none;
}
.menu-mobile {
    margin-right: 10px;
}

.nav-item {
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 20px;
    letter-spacing: -0.01em;
    color: #282A33;
    padding: 30px 16px;
    margin: auto 16px;
    position: relative;
}

.nav-link {
    position: relative;
    transition: all ease-in-out 0.1s;
}

.selection {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    top: 70%;
    display: none;
}

.selection.active {
    display: block;
}

.nav-link:hover {
    font-weight: 500;
    z-index: 99;
}

.nav-link:hover .selection {
    display: block;
    color: #282A33;
}

.nav-btn-access {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    color: #282A33;
    padding: 14px 24px;
    width: 104px;
    height: 48px;
    border: 2px solid #282A33;
    border-radius: 32px;
    text-decoration: none;
    cursor: pointer;
    margin: auto 16px;
}

.nav-btn-access:hover {
    background-color: #ca1d80;
    border: 2px solid #FFFFFF;
    color: #FFFFFF;
}

@media (max-width: 992px) {
    .nav-item {
    padding: 10px 16px;
    box-shadow: 0px 0px 2px rgba(0, 0, 0, 0.05);
}

.navbar-nav {
    margin-top: 24px;
}
.nav-btn-access{
    margin: 0 auto;
    width: 80%;
}
.selection, .selection.active {
    display: none;
}
}

</style>
s