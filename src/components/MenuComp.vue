<template>
  <div class="MainMenu">
    <div class="menuList">
      <v-icon icon="mdi-menu" size="x-large"></v-icon>

      <div class="menuItem">
        <h3 class="menuLabel">Proyectos</h3>
        <v-icon class="menuIcon" icon="mdi-briefcase-account-outline" size="large"></v-icon>
      </div>

      <div class="menuItem">
        <h3 class="menuLabel">Experiencia</h3>
        <v-icon class="menuIcon" icon="mdi-badge-account-outline" size="large"></v-icon>
      </div>

      <div class="menuItem">
        <h3 class="menuLabel">Skills</h3>
        <v-icon class="menuIcon" icon="mdi-account-star-outline" size="large"></v-icon>
      </div>

      <div class="menuItem">
        <h3 class="menuLabel">Contacto</h3>
        <v-icon class="menuIcon" icon="mdi-mailbox-open" size="large"></v-icon>
      </div>
    </div>

    <div class="redes">
      <v-icon icon="mdi-github" size="x-large"></v-icon>
      <v-icon class="redesIcon" icon="mdi-linkedin" size="x-large"></v-icon>
    </div>
  </div>
</template>

<style scped>
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

.menuList {
  display: flex;
  flex-direction: column;
  align-items: end;
}

h3 {
  padding-top: 20px;
}

.redes {
  padding: 10px;
}

.redes .redesIcon {
  margin-left: 15px;
}

.menuItem {
  display: flex;
  align-items: center;
  padding-top: 15px;
}

h3 {
  padding: 0;
  margin: 0;
  margin-right: 5px;
}
</style>
