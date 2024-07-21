<template>
  <div class="MainMenu">
    <div class="menuList">
      <v-icon icon="mdi-menu" class="menuIcon"></v-icon>

      <div class="menuItem" @click="redirect('proyects')">
        <h3 class="menuLabel">Proyectos</h3>
      </div>

      <div class="menuItem" @click="redirect('experience')">
        <h3 class="menuLabel">Experiencia</h3>
      </div>

      <div class="menuItem" @click="redirect('skills')">
        <h3 class="menuLabel">Skills</h3>
      </div>

      <div class="menuItem" @click="redirect('contact')">
        <h3 class="menuLabel">Contacto</h3>
      </div>
    </div>

    <div class="redes">
      <v-icon icon="mdi-github" class="redIcon"></v-icon>
      <v-icon icon="mdi-linkedin" class="redIcon"></v-icon>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {
    redirect(path) {
      this.$router.push({ path: `/${path}`, replace: true })
    }
  }
}
</script>

<style scoped>
.MainMenu {
  width: 100%;
  height: 100%;
  color: white;

  display: flex;
  flex-direction: column;
  align-items: end;
  justify-content: space-between;

  padding: 10px;
}

.menuIcon {
  font-size: 30px !important;
}

.menuList {
  display: flex;
  flex-direction: column;
  align-items: end;
}

h3 {
  padding-top: 20px;
}

.redIcon {
  padding: 15px;
  font-size: 30px !important;
}

.redes {
  margin-left: 15px;
}

.menuItem {
  display: flex;
  align-items: center;
  padding-top: 25px;
}

h3 {
  padding: 0;
  margin: 0;
  margin-right: 5px;
}

h3:hover {
  font-size: 25px;
}

@media (min-width: 1024px) {
}

@media (min-width: 769px) and (max-width: 1023px) {
}

@media (max-width: 768px) {
  .MainMenu {
    width: 100%;
    height: 100%;
    color: white;

    display: flex;
    flex-direction: row-reverse;
    align-items: end;
    justify-content: space-between;

    padding: 5px;
  }

  .menuIcon {
    font-size: 25px !important;
  }

  .menuList {
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    justify-content: center;
    padding-bottom: 5px;
  }

  .menuItem {
    display: flex;
    align-items: center;
    justify-content: center;
    padding-top: 0;
  }

  h3 {
    padding: 0;
    margin: 0;
    margin-right: 5px;
    font-size: 12px;
  }

  .redIcon {
    padding: 10px;
    font-size: 20px !important;
  }

  .redes {
    margin-left: 5px;
    margin-bottom: 5px;
  }

  h3:hover {
    font-size: 12px;
  }
}
</style>
