<template>
  <main>
    <Jumbo/>
    <div class="container">
      <Comics/>
    </div>
  </main>
</template>

<script>
import Comics from "../sections/Comics.vue";
import Jumbo from "../sections/Jumbo.vue"

export default {
    name: "Main",
    components: {
      Jumbo,
      Comics
    }
}
</script>

<style lang="scss">
@import '../../assets/style/partials/variables.scss';

  main {
    background-color: $background-dark;

    .container {
      color: $text-light;
    }
  }
</style>