<template>
    <div class="Home">
        <header>
            <nav>
                <div class="menu-item">
                    <router-link to="/"><a href="#">Login</a></router-link>
                </div>
            </nav>
        </header>
     <ventanaerror />
        <div class="wrapper fadeInDown"> 
            <div id="formContent">
                <br /><br /><br />
                <form> 
                    <input
                        type="email"
                        id="login"
                        class="fadeIn second"
                        name="login"
                        placeholder="Correo Electronico"
                        required
                    />
                    <input
                        type="password"
                        id="password"
                        class="fadeIn third"
                        name="password"
                        placeholder="Contraseña"
                        required
                        minlength="8"
                    />
                <abbr title="Este campo es obligatorio" aria-label="required"></abbr>
                    <input 
                        type="submit"
                        class="fadeIn fourth"
                        value="Log In"
                       v-on:click="signIn" 
                    />
                    <input
                        type="submit"
                        class="fadeIn fourth"
                        value="Sign Up"
                        v-on:click="signUp"
                    />
                </form>

                <!-- Remind Passowrd -->
                <div id="formFooter">
                        <a class="underlineHover" href="#" v-on:click="password">
                            Forgot Password?</a>
                    <div id="components-demo">
                        <button-counter></button-counter>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Styles from '@/css/Login.css'
import ventanaerror from './VentanaError';
export default {
    name: "login",
    components: {
        ventanaerror,
    },
    methods: {
        signIn: function () {
            <button></button>
            this.$router.push("/home");

    
            // Codigo para logearse 
        },
        signUp: function () {
            this.$router.push("/register");
        // Codigo para registrarse
        },

        password: function (){
            this.$router.push("/password");
            // Forgot Password
        }
        },
    };
</script>
