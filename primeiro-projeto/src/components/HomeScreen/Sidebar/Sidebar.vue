<template>
  <div class="container">
    <div>
      <ButtonSidebar />
    </div>
    <div class="container-link">
      <a href="">Contatos</a>
      <a href="">Info</a>
      <a href="">Loja</a>
      <a href="">Locais</a>
    </div>
  </div>
</template>


<script>
import ButtonSidebar from "./ButtonSidebar.vue";

export default {
  name: "Sidebar",
  components: {
    ButtonSidebar,
  },
};
</script>


<style scoped>
:root {
  --orange: #f78b00;
  --blue: #00285f;
  --gray: #ededed;
}

.container {
  width: 300px;
  height: 100%;
  top: 0;
  left: 0px;

  position: fixed;
  z-index: 9;
  overflow: hidden;

  background-color: red;
  position: fixed;
}
.container-link {
  display: flex;

  flex-direction: column;
  align-items: center;
  justify-content: center;
}

a {
  margin-top: 3%;
  text-decoration: none;
  
  color: var(--blue);
}
</style>