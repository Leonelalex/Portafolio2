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
  width: 35%;
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
  font-size: 60px;
  font-weight: 600;
  margin: 0;
  padding: 0;
}

h3 {
  font-size: 35px;
  margin: 0;
  padding: 0;
}
</style>
