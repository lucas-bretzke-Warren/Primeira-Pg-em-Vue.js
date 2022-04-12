<template>
  <div class="Footer-center">
    <div class="Single-item">
      <h3>Company</h3>
      <p>
        About <br />
        Contact
      </p>
    </div>

    <div class="Single-item">
      <h3>Rental</h3>
      <p>
        Self-Drive <br />
        Chauffer-Driven <br />
        Help
      </p>
    </div>

    <div class="Single-item">
      <h3>Stay-connect</h3>
      <img :src="instagram" class="img-instagram" />
      <img :src="faccebok" class="img-instagram" />
    </div>

    <div class="Single-item">
      <h3>Contacts US</h3>
      <p>
        +55 47 9 8403-6489 <br />
        contato@gmail.com.br <br />
        Nome da Rua, Blumenau SC
      </p>
    </div>
  </div>
</template>


<script>
export default {
  name: "Footer",
  data() {
    return {
      instagram: "/img/instagram.png",
      faccebok: "/img/facebook.png",
    };
  },
};
</script>


<style>
:root {
  --orange: #f78b00;
  --blue: #00285f;
  --gray: #ededed;
}

.Footer-center {
  width: 100%;
  height: 150px;

  padding: 0px 0px 40px;
  margin-top: 50px;

  display: flex;
  align-items: center;
  justify-content: space-between;

  background-color: var(--orange);
}

.Single-item {
  padding: 50px;
  text-align: left;

  color: white;
}

.Single-item p {
  font-size: 15px;
}

.Single-item h3 {
  margin-bottom: 10px;
}

.img-instagram {
  width: 35px;
  height: auto;

  margin: 3px;
}
</style>