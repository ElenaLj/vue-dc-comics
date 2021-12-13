<template>
  <main>
    <div class="container">
      ******  CONTENT GOES HERE ******
    </div>
  </main>
</template>

<script>
export default {
    name: "Main"
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';

  main {
    height: 100px;
    background-color: $background-dark;

    .container {
      color: $text-light;
    }
  }
</style>