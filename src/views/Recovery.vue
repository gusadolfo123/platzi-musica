<template>
  <section class="recovery">
    <section class="recovery__container">
      <h2>Recuperar Contraseña</h2>
      <form class="recovery__container--form">
        <input type="text" class="input" placeholder="Correo" />
        <button class="button">Enviar</button>
      </form>
      <p class="recovery__container--login">
        <a href="/login">Iniciar Sesion</a>
      </p>
    </section>
  </section>
</template>

<script>
export default {
  name: "recovery"
};
</script>

<style scoped>
.recovery {
  background: linear-gradient(#21c08b, #ab88ff);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 30px 30px;
  min-height: calc(100vh - 200px);
}
.recovery__container {
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
.recovery__container--form {
  display: flex;
  flex-direction: column;
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
.recovery__container--login {
  text-align: center;
}
.recovery__container--login a {
  text-decoration: none;
  color: whitesmoke;
  font-weight: bold;
  letter-spacing: 1px;
}
.recovery__container--login a:hover {
  text-decoration: underline;
}
</style>