<template>
  <footer>
    <div class="container footer">

      <!-- footer top section -->
      <div class="footer-top">

        <div>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics pic">
          <span>digital comics</span>
        </div>

        <div>
          <img src="../assets/img/buy-comics-merchandise.png" alt="Merch">
          <span>dc merchandise</span>
        </div>

        <div>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="Subscriptions">
          <span>subscription</span>
        </div>

        <div>
          <img src="../assets/img/buy-comics-shop-locator.png" alt="Shop Locator">
          <span>comic shop locator</span>
        </div>

        <div>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">
          <span>dc power visa</span>
        </div>

      </div>
      <!-- /footer top section -->

      <!-- footer middle section -->
      <div class="footer-middle"></div>
      <!-- /ooter middle section -->

      <!-- footer bottom section -->
      <div class="footer-bottom"></div>
      <!-- /footer bottom section -->
    </div>
  </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';

  footer {
    background-color: $background-blue; 

    .footer-top {
      display: flex;
      justify-content: center;
      color: $text-light;
      font-size: 14px;
      text-transform: $text-uppercase;

      div {
        display: flex;
        align-items: center;
        padding: 20px;

        img {
          height: 50px;
          max-width: 50px;
          margin-right: 8px;
        }
      }
    }
  }
</style>