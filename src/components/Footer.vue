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
      <div class="footer-middle">

        <div class="container">
          <!-- footer links section -->
          <div class="links">

            <div class="col-one">
              <!-- first column links sections -->
              <h3>dc comics</h3>
              <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
              </ul>

              <h3>shop</h3>
              <ul>
                <li><a href="#">Shop DC</a></li>
                <li><a href="#">Shop DC Collectibles</a></li>
              </ul>
              <!-- /first column links section -->
            </div>

            <div class="col-two">
              <!-- first column links sections -->
              <h3>DC</h3>
              <ul>
                <li><a href="#">Terms Of Use</a></li>
                <li><a href="#">Privacy policy (New)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">Talent Workshops</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
              </ul>
              <!-- /first column links section -->
            </div>

            <div class="col-three">
              <!-- first column links sections -->
              <h3>sites</h3>
              <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
              </ul>
              <!-- /first column links section -->
            </div>
          </div>
          <!-- /footer links section -->
        </div>

        <!-- footer logo image -->
        <!-- <img src="../assets/img/dc-logo-bg.png" alt="DC logo big"> -->
        <!-- /footer logo image -->

      </div>
      <!-- /footer middle section -->

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

  .footer-middle {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;

      .links  {
        display: flex;
        padding: 25px;

          .col-one, 
          .col-two, 
          .col-three {
            margin: 0 25px;
          }

          li a {
            color: $text-grey;
            font-size: 13px;
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