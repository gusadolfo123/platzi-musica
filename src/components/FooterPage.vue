<template>
  <footer class="footer">
    <a href="/">Terminos de uso</a>
    <a href="/">Declaracion de privacidad</a>
    <a href="/">Centro de ayuca</a>
  </footer>
</template>

<script>
export default {
  name: "FooterPage"
};
</script>

<style scoped>
.footer {
  display: flex;
  align-items: center;
  height: 100px;
  width: 100%;
  background-color: #ab88ff;
}
.footer a {
  color: whitesmoke;
  cursor: pointer;
  font-size: 14px;
  text-decoration: none;
  padding-left: 14px;
}
.footer a:hover {
  text-decoration: underline;
}
@media only screen and (max-width: 600px) {
  .footer {
    align-items: flex-start;
    flex-direction: column;
  }
}
</style>