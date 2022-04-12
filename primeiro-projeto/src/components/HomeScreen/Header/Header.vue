<template>
  <header>
    <div class="content">
      <nav>
        <div class="logo"><ButtonSidebar /></div>

        <div>
          <a href="">Catalog</a>
          <a href="">About</a>
          <a href="">Features</a>
          <button>Login</button>
        </div>
      </nav>

      <HeaderBlock />
    </div>
  </header>
</template>

<script>
import ButtonSidebar from "../Sidebar/ButtonSidebar.vue";
import HeaderBlock from "./HeaderBlock";

export default {
  name: "Header",
  components: {
    HeaderBlock,
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

* {
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
  font-family: Roboto, sans-serif;
  outline: none;
}

body {
  padding: 0px;
  margin: 0px;
}

header {
  width: 100%;
  height: 500px;

  margin: 0px 0px 200px 0px;

  align-items: center;

  background-color: var(--orange);
}

.content {
  max-width: 1000px;
  min-width: 300px;

  margin: 0px auto;
  flex-direction: column;
}

nav {
  padding: 50px 0px;

  display: flex;

  justify-content: space-between;
  background-color: var(--orange);
}

.logo {
  display: flex;
  align-items: center;
  justify-content: center;

  font-size: 22px;
}

nav a {
  padding: 10px 20px;

  font-size: 16px;
  color: var(--blue);
  text-decoration: none;

  cursor: alias;
  transition: 0.5s;
}

nav a:hover {
  color: white;
}

nav button {
  padding: 10px 35px;

  font-size: 16px;
  color: var(--blue);

  cursor: pointer;
  border-radius: 5px;
  border: solid 1px black;
  background-color: var(--orange);
}

nav button:hover {
  transition: 0.5s;

  color: white;
  background-color: var(--blue);
}
</style>