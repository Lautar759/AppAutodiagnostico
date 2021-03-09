<template>
    <div class="Home">
        <div class="wrapper fadeInDown">
            <div id="formContent">
                <br /><br /><br />
                <form>
                    <h1>Autodiagnóstico</h1>
                    ¿Percibiste una marcada pérdida del olfato de manera
                    repentina?
                    <input
                        type="checkbox"
                        id="olfato"
                        name="answer"
                        value="Si" 
                    /><br />
                    ¿Percibiste una marcada pérdida del gusto (sabor de los
                    alimentos) de manera repentina?
                    <input
                        type="checkbox"
                        id="gusto"
                        name="answer"
                        value="Si"
                    /><br />
                    ¿Tenés tos?
                    <input
                        type="checkbox"
                        id="tos"
                        name="answer"
                        value="Si"
                    /><br />
                    ¿Tenés dolor de garganta?
                    <input
                        type="checkbox"
                        id="garganta"
                        name="answer"
                        value="Si"
                    /><br />
                    ¿Tenés dificultad respiratoria o falta de aire?
                    <input
                        type="checkbox"
                        id="aire"
                        name="answer"
                        value="Si"
                    /><br />
                    ¿Tenés dolor de cabeza?
                    <input
                        type="checkbox"
                        id="cabeza"
                        name="answer"
                        value="Si"
                    /><br />
                    ¿Tenés diarrea?
                    <input
                        type="checkbox"
                        id="diarrea"
                        name="answer"
                        value="Si"
                    /><br />
                    ¿Tenés vómitos?
                    <input
                        type="checkbox"
                        id="vomito"
                        name="answer"
                        value="Si"
                    /><br />
                    ¿Tenés dolor muscular?
                    <input
                        type="checkbox"
                        id="dolor"
                        name="answer"
                        value="Si"
                    /><br />
                </form>
                <router-link to="/home">
                    <input
                        type="submit"
                        class="fadeIn fourth"
                        value="Aceptar"
                    />
                </router-link>
            </div>
        </div>
    </div>
</template>

<script>
import Styles from '@/css/Diagnostico.css'
export default {
    name: "login",

    methods: {
        signUp: function () {
            //  Codigo para logearse
        },
    },
};
</script>
