<template>
  <div>
    <a @click="showNav"><strong>Projeto</strong>Vue.js</a>
    <p v-show="mostrar_Nav"><Sidebar/></p>
  </div>
</template>





<script>
import Sidebar from './Sidebar.vue';

export default {
  name: "ButtonSidebar",
  components: {Sidebar},
  data() {
      return{
          mostrar_Nav: false,
          Nav: Sidebar,
      }
  },
  methods: {
      showNav() {
          this.mostrar_Nav = !this.mostrar_Nav;
      }
  },
  props: {
    showNav: Boolean
  }
};
</script>




<style scoped>
:root {
  --orange: #f78b00;
  --blue: #00285f;
  --gray: #ededed;
}

a {
  color: var(--blue);
  cursor: pointer;
  transition: 1s;
}

a:hover {
  color: #fff;
}
</style>>

