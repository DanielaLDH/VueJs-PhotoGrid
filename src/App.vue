<template>
  <v-app> 
    <div class="top">
      <div class="avatar">
        <v-avatar size="100">
          <img
            src="https://picsum.photos/200/300"
            alt="John"
          >
        </v-avatar>
      </div>
      <div>
        <H3>Daniela's PhotoGrid</H3>
        <H5>I'm from Blumenau</H5>
      </div>
    </div>
    <v-main>
      <FotosIndex/>
    </v-main>
  </v-app>
</template>

<script>
import FotosIndex from './components/FotosIndex';

export default {
  name: 'App',

  components: {
    FotosIndex,
  },

  data: () => ({
    //
  }),
};
</script>

<style scoped>
.top{
  display: flex;
  justify-content:space-evenly;
  align-items: center;
  height: 20vh;
}
</style>