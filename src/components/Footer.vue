<template>
  <footer>
    <div class="container-footer">

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
      <div class="footer-bottom">

        <div class="container">

          <button>sign-up now!</button>

          <div>
            <span>follow us</span>
            <img src="../assets/img/footer-facebook.png" alt="facebook">
            <img src="../assets/img/footer-twitter.png" alt="twitter">
            <img src="../assets/img/footer-youtube.png" alt="youtube">
            <img src="../assets/img/footer-pinterest.png" alt="pinterest">
            <img src="../assets/img/footer-periscope.png" alt="periscope">
          </div>
        </div>

      </div>
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
  .footer-top {
    background-color: $background-blue; 
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

  .footer-bottom {
    background-color: $background-grey;

      .container {
        height: 100px;
      }

      button {
        border: 1px solid #0C7CEC;
        background-color: transparent;
        padding: 20px;
        color: $text-light;
        font-weight: $text-bold;
        text-transform: $text-uppercase;
      }

      div {
        display: flex;
        flex-grow: 1;
        justify-content: flex-end;
        align-items: center;

        span {
          color: $text-blue;
          text-transform: $text-uppercase;
          font-weight: $text-bold;
        }

        img {
          margin: 0 10px;
        }
      }
    }
</style>