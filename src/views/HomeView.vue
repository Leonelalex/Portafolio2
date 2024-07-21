<template>
  <div class="main">
    <img class="logoLR" :src="myLogo" alt="LR" />
    <img class="mainFoto" :src="foto" alt="Leonel Recinos foto" />
    <div class="titleBlock">
      <h1>LEONEL RECINOS</h1>
      <h3>DESARROLLADOR WEB</h3>
    </div>
  </div>
</template>

<script>
import foto from '@/assets/images/FotoWeb.png'
import myLogo from '@/assets/logos/LogoLRBlanco.png'

export default {
  data() {
    return {
      foto,
      myLogo
    }
  }
}
</script>

<style scoped>
.main {
  width: 100%;
  height: 100%;

  display: flex;
  align-items: center;
  justify-content: center;
}

.mainFoto {
  width: 45%;
  min-width: 550px;
  max-width: 750px;
}

.logoLR {
  position: absolute;
  width: 75px;
  height: 75px;
  top: 15px;
  left: 15px;
}

.titleBlock {
  color: white;
  position: absolute;
  top: 45%;
  left: 8%;
}

h1 {
  font-size: 55px;
  font-weight: 600;
  margin: 0;
  padding: 0;
}

h3 {
  font-size: 32px;
  margin: 0;
  padding: 0;
}

@media (min-width: 769px) and (max-width: 1023px) {
  h1 {
    font-size: 45px;
    font-weight: 500;
    margin: 0;
    padding: 0;
  }

  h3 {
    font-size: 25px;
    margin: 0;
    padding: 0;
  }

  .mainFoto {
    width: 40%;
    min-width: 500px;
  }
}

@media (max-width: 768px) {
  .mainFoto {
    width: 85%;
    min-width: unset;
  }

  .logoLR {
    position: absolute;
    width: 40px;
    height: 40px;
    top: 5px;
    left: 5px;
  }

  .titleBlock {
    color: white;
    position: absolute;
    top: 60%;
    left: 0;
    width: 100%;
    text-align: center;
  }

  h1 {
    font-size: 35px;
    font-weight: 500;
    margin: 0;
    padding: 0;
  }

  h3 {
    font-size: 20px;
    margin: 0;
    padding: 0;
  }
}
</style>
