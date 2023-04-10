<template>
    <nav class="navbar navbar-expand-lg mt-5">
        <div class="container a-box-shadow">
            <a href="/">
                <img alt="Logo Avaluo" class="logo" src="../assets/imgs/avaluo_logo.png" />
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
                aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        
                        <a class="nav-link" href="/">Inicio<img class="selection" src="../assets/imgs/Chevron.png" alt="Selection" width="15"></a>
                    </li>
                    <li class="nav-item">
                        
                        <a class="nav-link" href="/empresas">Empresas<img class="selection" src="../assets/imgs/Chevron.png" alt="Selection" width="15"></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="/personas">Personas<img class="selection" src="../assets/imgs/Chevron.png" alt="Selection" width="15"></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="/avaluo-certificado">Avalúo Certificado<img class="selection"
                                src="../assets/imgs/Chevron.png" alt="Selection" width="15"></a>

                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="/conexion-api">Conexión API
                            <img class="selection" src="../assets/imgs/Chevron.png" alt="Selection" width="15">
                        </a>
                    </li>
                </ul>
                <a class="nav-btn-access">Ingresar</a>
            </div>
        </div>
    </nav>
</template>



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
.nav-link.router-link-active .selection{
    display: block;
}
.nav-item:hover {
    color: black;
    font-weight: 500;
}
.nav-link:hover .selection{
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
}</style>