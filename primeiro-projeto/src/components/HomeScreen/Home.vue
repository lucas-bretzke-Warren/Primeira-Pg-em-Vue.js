<template>
  <div class="HOME">
    <Header />
    <InputPesquisa />
    <LinhaDeCarros/>
    <LinhaDeCarros/>
    <LinhaDeCarros/>
    <Sobre/>
    <Footer/>
    <DescricaoDaPagina/>
  </div>
</template>


<script>
import Header from "./Header/Header";
import InputPesquisa from "./InputPesquisa/Input.vue";
import LinhaDeCarros from './Carros/LinhaDeCarros.vue';
import Sobre from './Sobre.vue'
import Footer from './Footer/Footer.vue';
import DescricaoDaPagina from './Footer/DescricaoDaPagina'


export default {
  name: "HomeScreen",
  components: {
    Header,
    InputPesquisa,
    LinhaDeCarros,
    Sobre,
    Footer,
    DescricaoDaPagina,

  },
};
</script>


<style >
* {
  padding: 0px;
  margin: 0px;
}
</style>