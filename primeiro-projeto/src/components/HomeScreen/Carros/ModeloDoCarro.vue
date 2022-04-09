<template>
  <div class="modelCar">
    <img :src="AudiSupraTT" class="ImgCar" />
    <h2>{{ nome }}</h2>
    <p>{{ title }}</p>
    <button>I WANT THIS!</button>
  </div>
</template>

<script>
export default {
  name: "ModeloDeCarro",
  data() {
    return {
      AudiSupraTT: "/img/car-card.png",
      nome: "Audi Supra TT",
      title:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus.",
    };
  },
};
</script>






<style>

.modelCar {
  width: 27%;
  padding: 20px;

  border-radius: 5px;
  background-color: var(--gray);
}

.ImgCar {
  width: auto;
  max-width: 230px;
  padding: 10px;
}

.modelCar h2 {
  text-align: center;
  margin-bottom: 10px;
}

.modelCar p {
  margin-bottom: 15px;
}

.modelCar button {

  width: 100%;
  padding: 12px;

  font-size: 16px;
  color: white;

  border: none;
  border-radius: 5px;
  background-color: var(--blue);

  cursor: pointer;
  transition: 1s;
}

.modelCar button:hover {
  color: var(--blue);
  background-color: #4444;

  border-radius: 0px 200px 0px 200px;
}
</style>