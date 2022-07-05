<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="./assets/ghd-digital-logo-light-64px.png"
          transition="scale-transition"
        />
      </div>

      <v-spacer></v-spacer>
    </v-app-bar>

    <v-main>
      <UserGrid/>
    </v-main>
  </v-app>
</template>

<script>
import UserGrid from './components/UserGrid';

export default {
  name: 'App',

  components: {
    UserGrid,
  },

  data: () => ({
    //
  }),
};
</script>
