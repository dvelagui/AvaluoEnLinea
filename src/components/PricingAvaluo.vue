<template>
    <div class="pricing row justify-content-center px-2 p-md-5 text-center">
        <div class="col-12 col-md-3 mt-5 mt-md-0 p-0 p-md-0 ">
            <div class="flex-column justify-content-center features">
                <div class="pricing-border feature-head border-rounded-left">
                    <p class="plan-head_title"></p>
                    <p>Características</p>
                    <p class="plan-head_time"></p>

                </div>
                <div class="pricing-border feature-content">
                    <p>Tipo de reporte</p>
                </div>
                <div class="pricing-border feature-content">
                    <p>Reportes por mes</p>
                </div>
                <div class="pricing-border feature-content">
                    <p>Personalización del reporte</p>
                </div>
                <div class="pricing-border feature-content">
                    <p>Acceso a plataforma</p>
                </div>
                <div class="pricing-border feature-content">
                    <p>Avalúo certificado</p>
                </div>
                <div class="pricing-border feature-content">
                    <p>Cantidad de usuarios</p>
                </div>
                <div class="pricing-border feature-content border-rounded-left-bottom">
                    <p style="color: transparent">Planes</p>
                </div>
            </div>
        </div>
        <div class="col-12 col-md-3 mt-5 mt-md-0 px-2 p-md-0">
            <div class="d-flex flex-column justify-content-center plan">
                <div class="pricing-border plan-head">
                    <p class="plan-head_title">Plan Básico</p>
                    <p class="plan-head_price">$100.000/mes</p>
                    <p class="plan-head_time">$1’000.000/anual</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Reporte completo</p>
                </div>
                <div class="pricing-border plan-content">
                    <p><span>15 reportes </span>($6.700 c/u)</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Logotipo y colores</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Si</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>10% de descuento</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>5 usuarios</p>
                </div>
                <div class="pricing-border plan-content p-0 plan-footer">
                    <a href="" class="btn btn-primary">Seleccionar Plan Básico</a>
                </div>

            </div>
        </div>
        <div class="col-12 col-md-3 mt-5 mt-md-0 px-2 p-md-0">
            <div class="d-flex flex-column justify-content-center  plan">
                <div class="pricing-border plan-head">
                    <p class="plan-head_title">Plan Avanzado</p>
                    <p class="plan-head_price">$260.000/mes</p>
                    <p class="plan-head_time">$1’000.000/anual</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Reporte completo</p>
                </div>
                <div class="pricing-border plan-content">
                    <p><span>30 reportes</span> ($8.600 c/u)</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Logotipo y colores</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Si</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>10% de descuento</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>5 usuarios</p>
                </div>
                <div class="pricing-border plan-content p-0 plan-footer">
                    <a href="" class="btn btn-primary">Seleccionar Plan Avanzado</a>
                </div>
            </div>
        </div>
        <div class="col-12 col-md-3 mt-5 mt-md-0 px-2 p-md-0">
            <div class="d-flex flex-column justify-content-center plan">
                <div class="pricing-border plan-head border-rounded-right">
                    <p class="plan-head_title">Plan Profesional</p>
                    <p class="plan-head_price">$400.000/mes</p>
                    <p class="plan-head_time">$4’000.000/anual</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Reporte completo</p>
                </div>
                <div class="pricing-border plan-content">
                    <p><span>70 reportes</span> ($5.700 c/u)</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Logotipo y colores</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>Si</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>10% de descuento</p>
                </div>
                <div class="pricing-border plan-content">
                    <p>5 usuarios</p>
                </div>
                <div class="pricing-border plan-content p-0 border-rounded-right-bottom plan-footer">
                    <a href="" class="btn btn-primary">Seleccionar Plan Profesional</a>
                </div>
            </div>
        </div>
    </div>
    <!--  -->
</template>

<script setup>

</script>

<style lang="scss" scoped>
p {
    margin: 0;
}

.features {
    display: flex;
}

.pricing-border {
    border: 1px solid #E9EBF1;
}

.pricing {
    width: 100%;
    max-width: 1000px;
    margin: auto;
}

.features {
    text-align: left;
    background: #F7F9FD;
}


.plan-head,
.feature-head {
    padding: 20px 24px;
    height: 100%;
    min-height: 95px;
    max-height: 95px;
    background: #F7F9FD;

}

.feature-content,
.plan-content {
    padding: 16px 24px;
}

.feature-head p {
    font-weight: 600;
    font-size: 20px;
    line-height: 120%;
    letter-spacing: -0.01em;
    color: #282A33;
}



.feature-content p,
.plan-content p {
    font-weight: 400;
    line-height: 20px;
    letter-spacing: -0.01em;
    color: #282A33;
}

.feature-content p {
    font-size: 14px;
}

.plan-content p {
    font-size: 16px;
}


.plan-head_title {
    font-weight: 600;
    font-size: 20px;
    line-height: 100%;
    text-align: center;
    letter-spacing: -0.01em;
    color: #282A33;
}

.plan-head_price {
    font-weight: 600;
    font-size: 18px;
    line-height: 120%;
    text-align: center;
    letter-spacing: -0.01em;
    color: #CA1D80;
    margin: 5px auto 2px auto;
}

.plan-head_time {
    font-weight: 400;
    font-size: 12px;
    line-height: 120%;
    text-align: center;
    letter-spacing: -0.01em;
    color: #6B7082;
}

.plan-content span {
    color: #CA1D80;
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
    width: 90%;
    margin: 10px auto;
}

.border-rounded-left {
    border-radius: 16px 0 0 0;
}

.border-rounded-right {
    border-radius: 0 16px 0 0;
}

.border-rounded-left-bottom {
    border-radius: 0 0 0 16px;
}

.border-rounded-right-bottom {
    border-radius: 0 0 16px 0;
}

@media (max-width: 992px) {

    .features {
        display: none;
    }

    .border-rounded-left,
    .border-rounded-right,
    .border-rounded-left-bottom,
    .border-rounded-right-bottom {
        border-radius: 0;
    }
    .plan-head {
        border-radius: 16px 16px 0 0;
    }
    .plan-footer {
        border-radius:  0 0 16px 16px;
    }


}</style>