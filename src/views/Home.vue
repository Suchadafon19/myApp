<template>
  <div class="home">
   <!-- <img alt="Vue logo" src="../assets/logo.png">-->
    <Homepage />
    <Table/>
    <v-footer
      absolute
      class="font-weight-medium"
      id="footer"
    >
      <v-col
        class="text-center"
        cols="12"
      >
        <strong>Copyright © A.E.C. CANNING COMPANY LIMITED 2017</strong>
      </v-col>
    </v-footer>
  </div>
</template>

<script>
// @ is an alias to /src
import Homepage from '@/components/Homepage.vue'
import Table from '@/components/Table.vue'

export default {
  name: 'Home',
  components: {
    Homepage,
    Table
  }
}
</script>

<style scoped>
#footer {
  background-color: #041225;
}

.text-center{
  color:#ffffff;
}
</style>
