<template>
  <section class="main">
    <h2 class="main__title">Que quieres ver hoy?</h2>
    <input type="text" class="input" placeholder="Buscar..." />
    <carrousel></carrousel>
  </section>
</template>


<style scoped>
.main {
  background: linear-gradient(#21c08b, #ab88ff);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 30px 30px;
  min-height: calc(100vh - 200px);
}
.main__title {
  color: whitesmoke;
  font-size: 25px;
}
.input {
  background-color: rgba(255, 255, 225, 0.1);
  border: 2px solid white;
  border-radius: 25px;
  color: whitesmoke;
  font-family: "Muli", sans-serif;
  font-size: 16px;
  height: 50px;
  padding: 0px 20px;
  width: 70%;
}
::placeholder {
  color: whitesmoke;
}
</style>

<script>
import carrousel from "../components/Carrousel";

export default {
  name: "home",
  components: {
    carrousel
  }
};
</script>

