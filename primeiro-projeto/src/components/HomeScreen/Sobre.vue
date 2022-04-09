<template>
  <div class="center">
    <div class="Sobre">
      <div class="content-img">
        <img :src="ImgSobre" alt="" />
      </div>

      <div class="text">
        <h3>Join technology and mobility</h3>
        <br />
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae
          ut inventore magni repellendus ab ad itaque facere. A tenetur quam,
          nobis tempore illum laborum ipsa fuga, itaque possimus repellat ad
          perspiciatis, velit reiciendis eos facilis sapiente blanditiis quas
          officia hic beatae quibusdam! Quod eligendi porro possimus voluptatum
          ad ipsum sapiente soluta, maiores nobis tenetur adipisci officiis nisi
          illum quae natus nostrum tempora accusantium blanditiis? Rem nesciunt
          illum dolorum, perferendis quos consequatur suscipit cumque fugiat
          alias sint repellat qui adipisci error est distinctio doloribus labore
          sunt modi eos odio quibusdam dicta. Dignissimos voluptate illum
          possimus quo. Ducimus repellat doloribus quisquam quidem?
        </p>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Sobre",
  data() {
    return {
      ImgSobre: "/img/about.jpg",
    };
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

  margin: 0px auto;

border-radius: 5px;
  background-color: var(--gray);
}

.Sobre {
  height: 600px;
  display: flex;
}

.content-img {
  width: 50%;
  height: auto;

  justify-content: center;
}

.text {
  width: 50%;

  padding: 10% 70px 0px 0px;

  font-size: 18px;
  text-align: right;
}

.text p {
    color: rgba(77, 77, 77, 0.471);
}

.content-img img {
  width: 70%;
  height: 96%;

  margin: 10px;

  border-radius: 10px;
  background-color: #444;
}
</style>