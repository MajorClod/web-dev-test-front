<template>
  <v-row class="text-center">
    <v-col>
      {{id}}
    </v-col>
    <v-col>
      {{domain}}
    </v-col>
    <v-col>
      {{start_date}}
    </v-col>
  </v-row>
</template>

<script>
  export default {
    name: 'UserGridLine',
    props: ['id', 'domain', 'start_date']
  }
</script>

