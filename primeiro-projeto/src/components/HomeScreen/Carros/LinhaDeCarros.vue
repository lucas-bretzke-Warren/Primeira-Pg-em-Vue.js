<template>
  <div class="center">
    <div class="FaixaDeCarros">
      <ModeloDeCarro />
    </div>
  </div>
</template>


<script scoped>
import ModeloDeCarro from "./ModeloDoCarro.vue";

export default {
  name: "LinhaDeCarros",
 components: {
    ModeloDeCarro,
  },
};
</script>


<style scoped>
:root {
  --orange: #f78b00;
  --blue: #00285f;
  --gray: #ededed;
}

.center {
  max-width: 1000px;
  min-width: 300px;

  margin: 50px auto;

  border-radius: 5px;
}

.FaixaDeCarros {
  display: flex;
  align-items: center;
  justify-content: space-around;
}
</style>