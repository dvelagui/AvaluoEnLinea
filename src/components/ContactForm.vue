<template>
    <div class="contact-form mt-5 mb-5 px-2 px-md-0">
        <div class="row d-flex justify-content-center">
            <div class=" col-12 col-md-6">
                <img class="contact-form_img my-1" src="https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Farrow_right.svg?alt=media&token=1397e239-f6b6-4828-9c3b-1b45696d6415" alt="Contact">
                <h6 class="contact-form_title">Contáctanos</h6>
                <p class="contact-form_p">
                    Si tienes cualquier duda o comentario, escríbenos
                </p>
            </div>
        </div>


        <form @submit.prevent="sendContactForm">
            <div class="row g-3 d-flex justify-content-center mt-0 mt-md-1">
                <div class="col-12 col-md-3">
                    <label class="contact-form_label form-label" for="nameInput">Nombre</label>
                    <input class="contact-form_email form-control" type="text" name="nameInput" v-model="nameInput"
                        placeholder="Escribe tu nombre completo" />
                </div>
                <div class="col-12 col-md-3">
                    <label class="contact-form_label form-label" for="telInput">Celular</label>
                    <input class="contact-form_tel form-control" type="tel" name="telInput" v-model="telInput"
                        placeholder="Escribe tu numero de celular" />
                </div>
            </div>
            <div class="row g-3 d-flex justify-content-center mt-0 mt-md-1">
                <div class="col-12 col-md-3">
                    <label class="contact-form_label form-label" for="emailInput">Correo electrónico</label>
                    <input class="contact-form_email form-control" type="email" name="emailInput" v-model="emailInput"
                        placeholder="correoelectronico@email.com" />
                </div>
                <div class="col-12 col-md-3">
                    <label class="contact-form_label form-label" for="companyInput">Empresa (opcional)</label>
                    <input class="contact-form_tel form-control" type="text" name="conpanyInput" v-model="companyInput"
                        placeholder="Escribe el nombre de la empresa" />
                </div>
            </div>
            <div class="row g-3 d-flex justify-content-center mt-0 mt-md-1">
                <div class="col-12 col-md-6">
                    <label class="contact-form_label form-label" for="messageInput">Mensaje</label>
                    <textarea class="contact-form_tel form-control" name="messageInput" v-model="messageInput" cols="30"
                        rows="3" placeholder="Escribe tu mensaje..."></textarea>
                </div>
            </div>
            <div class="row g-3 d-flex justify-content-center mt-1">
                <div class="col-12 col-md-6">
                    <input type="checkbox" v-model="checkTerms" class="form-check-input" />
                    <label for="checkTerms" class="form-check-label ms-2">
                        Acepto Terminos y Condiciones</label>
                </div>
            </div>
            <div class="row g-3 d-flex justify-content-center mt-1">
                <div class="col-12 col-md-6">
                    <input class="btn btn-primary" type="submit" value="Enviar" />
                </div>
            </div>
        </form>
    </div>
</template>

<script setup>
import { ref } from "vue";

const nameInput = ref();
const telInput = ref();
const emailInput = ref();
const companyInput = ref();
const messageInput = ref();
const checkTerms = ref();

const sendContactForm = () => {
    alert(`
    
${nameInput.value}
${telInput.value}
${emailInput.value}
${companyInput.value}
${messageInput.value}
${checkTerms.value}

registro completo
    `);
}

</script>

<style lang="scss" scoped>

.contact-form_img {
    display: none;
}
.contact-form_title {
    font-weight: 600;
    font-size: 48px;
    line-height: 100%;
    letter-spacing: -0.01em;
    color: #000000;
  margin-left: -75px;

}
.contact-form_title::before {
  content:url('https://firebasestorage.googleapis.com/v0/b/quasar-chat-285ff.appspot.com/o/Avaluo%2Farrow_right.svg?alt=media&token=1397e239-f6b6-4828-9c3b-1b45696d6415');
  margin-right: 40px;
  display: inline;
}

.contact-form_p {
    font-weight: 400;
    font-size: 16px;
    line-height: 20px;
    letter-spacing: -0.01em;
    color: #6B7082;
}

.form-control {
    border: 2px solid #c1c6d5;
    border-radius: 4px;
    line-height: 2.5;
}

.btn {
    font-family: 'Source Sans Pro';
    border-radius: 32px;
    font-weight: 600;
    font-size: 16px;
    line-height: 18px;
    text-align: center;
    letter-spacing: -0.01em;
    color: #FFFFFF;
    padding: 14px 24px;

}
.form-check-input {
    border: 1px solid #ca1d80;
}


@media (max-width: 992px) {
    .contact-form_img {
    display: block;
    width: 30px;
    transform: rotate(90deg);
    margin: 0 auto;
    text-align: center;
}
.contact-form_title {
  margin: 0 auto;
  text-align: center;
font-size: 32px;
}
.contact-form_title::before {
  display: none;
}
.contact-form_p  {
    text-align: center;
    margin-top: 10px;
}
}

</style>