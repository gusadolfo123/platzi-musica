<template>
  <header class="header">
    <img class="header__img" src="../assets/logo-platzi.png" alt="asd" />
    <div class="header__menu">
      <div class="header__menu--profile">
        <img src="../assets/user.png" alt="asdsad" />
        <p>Perfil</p>
      </div>
      <ul>
        <li>
          <a href="/">Cuenta</a>
        </li>
        <li>
          <a href="/">Cerrar Sesion</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderPage"
};
</script>

<style scoped>
.header {
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #21c08b;
}
.header__img {
  width: 250px;
  /* margin-top: 10px;
  margin-left: 10px; */
}

.header__menu {
  margin-right: 30px;
}

.header__menu ul {
  display: none;
  list-style: none;
  padding: 0px;
  position: absolute;
  width: 100px;
  text-align: right;
  margin: 0px 0px 0px -14px;
}

.header__menu:hover ul,
ul:hover {
  display: block;
  cursor: pointer;
}

.header__menu li {
  margin: 10px 0px;
}

.header__menu li a {
  color: whitesmoke;
  text-decoration: none;
}

.header__menu li a:hover {
  text-decoration: underline;
}

.header__menu--profile {
  display: flex;
  align-items: center;
}

.header__menu--profile img {
  margin-right: 8px;
  width: 40px;
  height: 40px;
}

.header__menu--profile p {
  margin: 0px;
  color: whitesmoke;
}
</style>


