<template>
    <div class="Home">
        <div class="wrapper fadeInDown">
            <div id="formContent">
                <br /><br /><br />
                <form>
                    <input
                        type="text"
                        id="register"
                        class="fadeIn second"
                        name="register"
                        placeholder="Nombre y Apellido"
                    />
                    <input
                        type="text"
                        id="register"
                        class="fadeIn second"
                        name="register"
                        placeholder="Correo Electrónico"
                    />
                    <input
                        type="password"
                        id="password"
                        class="fadeIn third"
                        name="password"
                        placeholder="Contraseña"
                    />
                    <input
                        type="password"
                        id="repassword"
                        class="fadeIn third"
                        name="repassword"
                        placeholder="Confirmar contraseña"
                    /><br />
                    <br />
                    Sexo:
                    <select>
                        <option>Hombre</option>
                        <option>Mujer</option>
                        <option>Otro</option></select
                    ><br />
                    Fec. Nacimiento <input type="date" id="date" /><br />
                        <input v-onclick
                            type="submit"
                            class="fadeIn fourth"
                            value="Sign Up"
                            v-on:click="diagnostico"
                        />
                </form>
            </div>
        </div>
    </div>
</template>

<script>
import Styles from '@/css/Register.css'
export default {
  name: 'Register',

  methods:{   diagnostico: function () {
            this.$router.push("/diagnostico");
  }
}
};
</script>
