  <template>
    <v-app>
      <v-container>
    <v-row>
      <v-col v-for="character in characters" :key=character cols="12" lg="4" md="4" sm="4" >
           <v-card
    class="pa-2"
    max-width="400"
  >
    <v-img
      class="white--text align-end"
      height="200px"
      :src="character.imagen"
    >

    </v-img>
    <v-card-text class="text--primary">
      <div>{{character.nombre}}</div>
    </v-card-text>
  </v-card>
      </v-col>
    </v-row>
  </v-container>
    </v-app>
  </template>


  <script>

export default {
  name: 'App',
  data: () => ({
   characters: [
          {
          'id': 1,
          'nombre': 'Morty',
          'imagen': 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
          },
          {
          'id': 2,
          'nombre': 'Rick',
          'imagen': 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
          },
          {
          'id': 3,
          'nombre': 'Summer',
          'imagen': 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'
          },
          {
          'id': 4,
          'nombre': 'Beth',
          'imagen': 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'
          },
          {
          'id': 5,
          'nombre': 'Jerry',
          'imagen': 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'
          }
   ]
  })
};
</script>
