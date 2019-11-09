<template>
  <section class="login">
    <section class="login__container">
      <h2>Iniciar Sesion</h2>
      <form class="login__container--form">
        <input type="text" class="input" placeholder="Correo" />
        <input type="password" class="input" placeholder="Contraseña" />
        <button class="button">Iniciar Session</button>
        <div class="login__container--remember-me">
          <label for="box1">
            <input type="checkbox" class id="box1" value="Checkbox" /> Recuerdame
          </label>
          <a href="/recovery">Olvide Contraseña</a>
        </div>
      </form>
      <section class="login__container--social-media">
        <div>
          <img src="../assets/google-icon.png" alt="logo google" />
          Inicia Session con Google
        </div>
        <div>
          <img src="../assets/twitter-icon.png" alt="logo twiiter" />
          Inicia Session con Twitter
        </div>
      </section>
      <p class="login_container--register">
        No tienes ninguna cuenta?
        <a href="/register">Registrate</a>
      </p>
    </section>
  </section>
</template>

<script>
export default {
  name: "login"
};
</script>

<style scoped>
.login {
  background: linear-gradient(#21c08b, #ab88ff);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 30px 30px;
  min-height: calc(100vh - 200px);
}
.login__container {
  /* background: #3a3a3a; */
  background-color: rgba(255, 255, 255, 0.1);
  border: 2px solid whitesmoke;
  border-radius: 40px;
  color: whitesmoke;
  padding: 60px 68px 40px;
  min-height: 700px;
  width: 300px;
  display: flex;
  justify-content: space-around;
  flex-direction: column;
}
.login__container--form {
  display: flex;
  flex-direction: column;
}
.login__container--form label {
  font-size: 14px;
}
.login__container--remember-me {
  color: whitesmoke;
  display: flex;
  justify-content: space-between;
  margin-top: 10px;
}
.login__container--remember-me a {
  color: whitesmoke;
  font-size: 14px;
  text-decoration: none;
}
.login__container--remember-me a:hover {
  text-decoration: underline;
}
.login__container--social-media > div {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 14px;
  margin-bottom: 10px;
  padding: 5px 0px;
  border-radius: 25px;
  cursor: pointer;
}
.login__container--social-media > div > img {
  width: 30px;
  height: 30px;
  margin-right: 10px;
}
.login__container--social-media > div:nth-child(1) {
  background-color: #dd4b39;
}
.login__container--social-media > div:nth-child(2) {
  background-color: #1da1f2;
}
.login_container--register {
  text-align: center;
  font-size: 14px;
}
.login_container--register a {
  color: whitesmoke;
  font-size: 16px;
  font-weight: bold;
  text-decoration: none;
}
.login_container--register a:hover {
  text-decoration: underline;
}
.input {
  background-color: transparent;
  border-left: 0px;
  border-right: 0px;
  border-top: 0px;
  border-bottom: 2px solid whitesmoke;
  font-family: "Muli", sans-serif;
  font-size: 16px;
  margin-bottom: 20px;
  padding: 0px 20px;
  outline: none;
  height: 40px;
  color: whitesmoke;
}
::placeholder {
  color: whitesmoke;
}
.button {
  background-color: rgba(255, 255, 255, 0.2);
  border: none;
  border-radius: 25px;
  color: whitesmoke;
  cursor: pointer;
  font-family: "Muli", sans-serif;
  font-size: 16px;
  font-weight: bold;
  letter-spacing: 1px;
  height: 50px;
  margin: 10px 0px;
}
</style>