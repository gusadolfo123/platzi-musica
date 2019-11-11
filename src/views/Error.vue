<template>
  <section class="error">
    <section class="error__container">
      <h1 class="error_container__title">Page Not Found</h1>
      <img src="../assets/404.png" alt="error 404" class="error__container--img" />
      <p class="error_container__detail">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aceius.
        <a href="/">Go Home</a>
      </p>
    </section>
  </section>
</template>

<script>
export default {
  name: "error"
};
</script>

<style scoped>
.error {
  background: linear-gradient(#21c08b, #ab88ff);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 30px 30px;
  min-height: calc(100vh - 200px);
}
.error__container {
  width: 400px;
  height: 400px;
  text-align: center;
}
.error_container__title {
  color: whitesmoke;
  letter-spacing: 2px;
}
.error__container img {
  width: 300px;
}
.error_container__detail {
  color: whitesmoke;
}
.error_container__detail a {
  text-decoration: none;
  font-weight: bold;
}
.error_container__detail a:hover {
  text-decoration: underline;
}
</style>