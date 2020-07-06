<template>
    <div>
        <v-card class="table"> 
            <v-data-table
            :headers="headers"
            :items="desserts"
            :items-per-page="5"
            class="elevation-1"
            ></v-data-table>
        </v-card>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        pagination: {},
        headers: [
          {
            text: 'NET WEIGHT (g.)',
            align: 'start',
            sortable: false,
            value: 'WEIGHT',
          },
          { text: 'NET WEIGHT (2)', value: 'WEIGHT2' },
          { text: 'DRAIN WEIGHT', value: 'DRAIN' },
          { text: 'CAN SIZE', value: 'SIZE' },
          { text: 'CANS/CARTON', value: 'CARTON' },
          { text: 'CANS/20’FCL (Normal Lid)', value: 'Lid' },
          { text: 'CANS/20’FCL (EOE)', value: 'EOE' },
        ],
        desserts: [
          {
            WEIGHT: '50',
            WEIGHT2: 140,
            DRAIN: 159,
            SIZE: 60,
            CARTON: 24,
            Lid: 500,
            EOE: '1%',
          },
          {
            WEIGHT: '60',
            WEIGHT2: 200,
            DRAIN: 300,
            SIZE: 80,
            CARTON: 24,
            Lid: 2400,
            EOE: '1%',
          },
          {
             WEIGHT: '70',
            WEIGHT2: 140,
            DRAIN: 159,
            SIZE: 6.0,
            CARTON: 24,
            Lid: 2400,
            EOE: '1%',
          },
          {
             WEIGHT: '80',
            WEIGHT2: 140,
            DRAIN: 159,
            SIZE: 6.0,
            CARTON: 24,
            Lid: 2100,
            EOE: '1%',
          },
          {
             WEIGHT: '90',
            WEIGHT2: 140,
            DRAIN: 159,
            SIZE: 6.0,
            CARTON: 24,
            Lid: 2100,
            EOE: '1%',
          },
          {
             WEIGHT: '100',
            WEIGHT2: 140,
            DRAIN: 159,
            SIZE: 6.0,
            CARTON: 24,
            Lid: 2000,
            EOE: '1%',
          },
          {
            WEIGHT: '120',
            WEIGHT2: 140,
            DRAIN: 159,
            SIZE: 6.0,
            CARTON: 24,
            Lid: 1800,
            EOE: '1%',
          },
          {
            WEIGHT: '111',
            WEIGHT2: 140,
            DRAIN: 159,
            SIZE: 6.0,
            CARTON: 24,
            Lid: 3600,
            EOE: '1%',
          },
        ],
      }
    }
  }
</script>

<style>
.table{
    margin-bottom: 50px;
}
</style>