<template>
  <section class="register">
    <section class="register__container">
      <h2>Registrarse</h2>
      <form class="register__container--form">
        <input type="text" class="input" placeholder="Nombre" />
        <input type="email" class="input" placeholder="Correo" />
        <input type="password" autocomplete="false" class="input" placeholder="Contraseña" />
        <button class="button">Registrarse</button>
      </form>
      <p class="register__container--login">
        <a href="/login">Iniciar Sesion</a>
      </p>
    </section>
  </section>
</template>

<script>
export default {
  name: "Register"
};
</script>

<style>
.register {
  background: linear-gradient(#21c08b, #ab88ff);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 30px 30px;
  min-height: calc(100vh - 200px);
}
.register__container {
  border: 2px solid whitesmoke;
  border-radius: 40px;
  display: flex;
  justify-content: space-around;
  flex-direction: column;
  background: rgba(255, 255, 255, 0.1);
  min-height: 700px;
  width: 300px;
  padding: 0px 30px;
  padding: 60px 68px 40px;
  color: whitesmoke;
}
.register__container--form {
  display: flex;
  flex-direction: column;
}
.input {
  background: transparent;
  color: whitesmoke;
  font-family: "Muli", sans-serif;
  font-size: 16px;
  height: 40px;
  padding: 0px 20px;
  margin-bottom: 20px;
  border-left: 0px;
  border-right: 0px;
  border-top: 0px;
  border-bottom: 2px solid whitesmoke;
  outline: none;
}
::placeholder {
  color: whitesmoke;
}
.button {
  background-color: rgba(255, 255, 255, 0.4);
  border: none;
  color: whitesmoke;
  font-family: "Muli", sans-serif;
  font-size: 16px;
  font-weight: bold;
  letter-spacing: 1px;
  height: 50px;
  margin: 10px 0px;
  border-radius: 25px;
}
.register__container--login {
  text-align: center;
}
.register__container--login a {
  text-decoration: none;
  color: whitesmoke;
  font-weight: bold;
  letter-spacing: 1px;
}
.register__container--login a:hover {
  text-decoration: underline;
}
</style>