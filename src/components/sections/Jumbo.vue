<template>
  <div class="jumbo">
      <img src="../../assets/img/jumbotron.jpg" alt="Jumbotron">
  </div>
</template>

<script>
export default {
    name: "Jumbo"
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss'; //if used

    .jumbo  {
        img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            object-position: center top;
        }
    }
    
</style>