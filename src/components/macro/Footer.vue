<template>
  <footer>
    <div class="container-footer">

      <!-- footer top section -->
      <div class="footer-top">

        <div v-for="(menu, index) in leafMenu" :key="index">
          <img :src="require(`../../assets/img/${menu.src}`)" :alt="menu.alt">
          <span>{{menu.text}}</span>
        </div>

        <!-- <div>
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
        </div> -->

      </div>
      <!-- /footer top section -->

      <!-- footer middle section -->
      <div class="footer-middle">

        <div class="container">
          <!-- footer links section -->
          <div class="links">

            <div class="col-one">
              <h3>dc comics</h3>
              <ul>
                <li v-for="(link, index) in linksComics" :key="index"><a :href="link.url">{{link.title}}</a></li>
              </ul>

              <h3>shop</h3>
              <ul>
                <li v-for="(link, index) in linksShop" :key="index"><a :href="link.url">{{link.title}}</a></li>
              </ul>
            </div>

            <div class="col-two">
              <h3>DC</h3>
              <ul>
                <li v-for="(link, index) in linksOther" :key="index"><a :href="link.url">{{link.title}}</a></li>
              </ul>
            </div>

            <div class="col-three">
              <h3>sites</h3>
              <ul>
                <li v-for="(link, index) in linksSites" :key="index"><a :href="link.url">{{link.title}}</a></li>
              </ul>
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
          
          <!-- socials -->
          <div class="socials">
            <span>follow us</span>
            <div v-for="(social, index) in socials" :key="index">
              <img :src="require(`../../assets/img/${social.src}`)" :alt="social.alt">
            </div>
          </div>
          <!-- /socials -->
        </div>

      </div>
      <!-- /footer bottom section -->
    </div>
  </footer>
</template>

<script>
export default {
    name: "Footer",
    data() {
      return {
        leafMenu: [
          {
            text: "digital comics",
            src: "buy-comics-digital-comics.png",
            alt: "Digital Comics pic"
          },
          {
            text: "dc merchandise",
            src: "buy-comics-merchandise.png",
            alt: "Merch"
          },
          {
            text: "subscription",
            src: "buy-comics-subscriptions.png",
            alt: "Subscriptions"
          },
          {
            text: "comic shop locator",
            src: "buy-comics-shop-locator.png",
            alt: "Shop Locator"
          },
          {
            text: "dc power visa",
            src: "buy-dc-power-visa.svg",
            alt: "DC Power Visa"
          }
        ], 
        linksComics: [
          {
            title: "Characters",
            url: "#"
          },
          {
            title: "Comics",
            url: "#"
          },
          {
            title: "Movies",
            url: "#"
          },
          {
            title: "TV",
            url: "#"
          },
          {
            title: "Games",
            url: "#"
          },
          {
            title: "Videos",
            url: "#"
          },
          {
            title: "News",
            url: "#"
          }
        ],
        linksShop: [
          {
            title: "Shop DC",
            url: "#"
          },
          {
            title: "Shop DC Collectibles",
            url: "#"
          }
        ],
        linksOther: [
          {
            title: "Terms Of Use",
            url: "#"
          },
          {
            title: "Privacy policy (New)",
            url: "#"
          },
          {
            title: "Ad Choices",
            url: "#"
          },
          {
            title: "Advertising",
            url: "#"
          },
          {
            title: "Jobs",
            url: "#"
          },
          {
            title: "Subscriptions",
            url: "#"
          },
          {
            title: "Talent Workshops",
            url: "#"
          },
          {
            title: "CPSC Certificates",
            url: "#"
          },
          {
            title: "Ratings",
            url: "#"
          },
          {
            title: "Shop Help",
            url: "#"
          },
          {
            title: "Contact Us",
            url: "#"
          }
        ],
        linksSites: [
          {
            title: "DC",
            url: "#"
          },
          {
            title: "MAD Magazine",
            url: "#"
          },
          {
            title: "DC Kids",
            url: "#"
          },
          {
            title: "DC Universe",
            url: "#"
          },
          {
            title: "DC Power Visa",
            url: "#"
          }
        ],
        socials: [
          {
            src: "footer-facebook.png",
            alt: "facebook"
          },
          {
            src: "footer-twitter.png",
            alt: "twitter"
          },
          {
            src: "footer-youtube.png",
            alt: "youtube"
          },
          {
            src: "footer-pinterest.png",
            alt: "pinterest"
          },
          {
            src: "footer-periscope.png",
            alt: "periscope"
          }
        ]
      }
    }
}
</script>

<style lang="scss">
@import '../../assets/style/partials/variables.scss';
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
    background-image: url(../../assets/img/footer-bg.jpg);
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

      .socials {
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