<template>
  <v-container fluid>
    <UserGridLine v-for="account, i in accounts" :key="i" :id="account.id" :domain="account.domain"
      :start_date="account.start_date">
    </UserGridLine>
  </v-container>
</template>

<script>

import UserGridLine from './UserGridLine.vue'

export default {
  name: 'UserGrid',
  components: { UserGridLine },
  data: () => ({
    accounts: [{
        "id": 1,
        "domain": "ghd.com",
        "start_date": "2021-04-23"
    },
    {
        "id": 2,
        "domain": "linkedin.com",
        "start_date": "2021-03-29"
    },],
  }),
  mounted() {
  },
}
</script>

<style scoped>
.grid-header {
  background-color: lightgray;
}
</style>