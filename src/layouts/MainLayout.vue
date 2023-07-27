<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar style="background-color: #3F51B5;">
        <q-btn flat dense round icon="menu" aria-label="Menu" @click="toggleLeftDrawer" />

        <q-toolbar-title style="color: #f5f5f5;"> Quasar App </q-toolbar-title>

        <div style="color: #f5f5f5;">Quasar v{{ $q.version }}</div>
      </q-toolbar>
    </q-header>

    <q-drawer v-model="leftDrawerOpen" show-if-above bordered>
      <q-list>
        <q-item-label header> Menu </q-item-label>
        <div class="row justify-center">
          <q-avatar class="q-ma-md" size="200px">
            <img src="../img/LogoMilton.jpeg" spinner-color="white" />
          </q-avatar>
        </div>
        <EssentialLink v-for="link in essentialLinks" :key="link.title" v-bind="link" />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import EssentialLink from "components/EssentialLink.vue";

const linksList = [
  {
    title: "Pagina Principal",
    caption: "Informações Principais",
    icon: "search",
    transacoes: "/",
  },
  {
    title: "Aulas",
    caption: "Repositorio de aulas",
    icon: "school",
    transacoes: "videos",
  },
];

import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",

  components: {
    EssentialLink,
  },

  setup() {
    const url = ref('https://picsum.photos/500/300');
    const leftDrawerOpen = ref(false);

    return {
      url,
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
});
</script>
l
