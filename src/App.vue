<template>
  <v-app>
    <div>
      <v-toolbar color="blue lighten-2">
        <v-toolbar-title>Arquitectura C-S</v-toolbar-title>

        <div class="flex-grow-1"></div>

        <v-toolbar-items>
          <v-btn text :to="{name: 'antecedentes'}">Antecedentes</v-btn>
          <v-btn text :to="{name: 'tipos'}">Tipos</v-btn>
          <v-btn text :to="{name: 'elementos'}">Elementos</v-btn>
        </v-toolbar-items>

        <template v-if="$vuetify.breakpoint.smAndUp">
          <v-btn icon :to="{name: 'home'}">
            <v-icon>mdi-anchor</v-icon>
          </v-btn>
        </template>
      </v-toolbar>
    </div>
    <v-content>
      <router-view />
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    //
  })
};
</script>
