<template>
  <v-app>
    <div class="mainPage">
      <div class="content">
        <RouterView />
      </div>
      <div class="menu">
        <MainMenu />
      </div>
    </div>
  </v-app>
</template>

<script>
import { RouterView } from 'vue-router'
import MainMenu from '@/components/MenuComp.vue'

export default {
  components: { RouterView, MainMenu }
}
</script>

<style>
body {
  background-color: black;
  font-family: 'Roboto Serif', sans-serif;
}

.mainPage {
  width: 100%;
  height: 100%;
  display: flex;
}

.content {
  width: 100%;
  height: 100%;
  background-color: black;
}

.menu {
  width: 250px;
  height: 100%;
  max-width: 300px;
  background-color: black;
}

#app {
  height: 100%;
  width: 100%;
  max-width: none;
  padding: 0;
  margin: 0;
  display: flex;
}

@media (min-width: 1024px) {
  #app {
    height: 100%;
    width: 100%;
    max-width: none;
    padding: 0;
    margin: 0;
    display: flex;
  }
}

@media (max-width: 768px) {
  #app {
    height: 100%;
    width: 100%;
    max-width: none;
    padding: 0;
    margin: 0;
    display: flex;
  }

  .mainPage {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
  }

  .content {
    width: 100%;
    height: 100%;
    background-color: black;
  }

  .menu {
    height: 100px;
    width: 100%;
    max-width: none;
    background-color: black;
  }
}
</style>
