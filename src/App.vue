<template>
  <SearchComponent />
  <DetailsComponent />
</template>

<script>
import SearchComponent from '@/components/SearchComponent.vue'
import DetailsComponent from '@/components/DetailsComponent.vue'

export default {
  name: 'App',
  components: {
    SearchComponent,
    DetailsComponent
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;700&display=swap');

#app {
  font-family: Rubik, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  color: hsl(0, 0%, 17%);
}

body {
  margin: 0;
}

h1, h2, h3 {
  font-weight: 500;
}

p {
  font-size: 18px;
}

</style>
