<template>
  <footer>
    <div class="footer-up">
      <div class="container90 up">
        <div class="footer-link">

          <FooterMenu :title="'DC COMICS'" :urls="DcComics" />

          <FooterMenu :title="'DC'" :urls="DC"/>

          <FooterMenu :title="'SITES'" :urls="Sites"/>

          <FooterMenu :title="'SHOP'" :urls="Shop"/>

        </div>

        <div class="big-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>
    
    <div class="social-section">
      <div class="container90">
        <h4 class="subscribe"><a href="#"> SIGN-UP NOW!</a></h4>
        <div class="social-icon">
          <h4 class="follow">
            <a href="#">FOLLOW US</a>
          </h4>
          <ul>
            <li>
              <a href="#">
                <img src="../assets/img/footer-facebook.png" alt="Facebook">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-twitter.png" alt="Twitter">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-youtube.png" alt="YouTube">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-periscope.png" alt="Periscope">
              </a>
            </li>
          </ul>
        </div>
      </div>
      
    </div>

  </footer>
</template>

<script>
import FooterMenu from './FooterMenu.vue';

export default {
    name: 'MyFooter',
    components: {
      FooterMenu
    },
    data() {
      return {
        DcComics: [
          {
            url: '#',
            text: 'Characters'
          },
          {
            url: '#',
            text: 'Comics'
          },
          {
            url: '#',
            text: 'Movies'
          },
          {
            url: '#',
            text: 'TV'
          },
          {
            url: '#',
            text: 'Games'
          },
          {
            url: '#',
            text: 'Videos'
          },
          {
            url: '#',
            text: 'News'
          }
        ],
        DC: [
          {
            url: '#',
            text: 'Terms Of Use'
          },
          {
            url: '#',
            text: 'Privacy policy (New)'
          },
          {
            url: '#',
            text: 'Ad Choices'
          },
          {
            url: '#',
            text: 'Advertising'
          },
          {
            url: '#',
            text: 'Jobs'
          },
          {
            url: '#',
            text: 'Subscriptions'
          },
          {
            url: '#',
            text: 'Talent Workshops'
          },
          {
            url: '#',
            text: 'CPSC Certificates'
          },
          {
            url: '#',
            text: 'Ratings'
          },
          {
            url: '#',
            text: 'Shop Help'
          },
          {
            url: '#',
            text: 'Contact Us'
          }
        ],
        Sites: [
          {
            url: '#',
            text: 'DC'
          },
          {
            url: '#',
            text: 'MAD Magazine'
          },
          {
            url: '#',
            text: 'DC Kids'
          },
          {
            url: '#',
            text: 'DC Universe'
          },
          {
            url: '#',
            text: 'DC Power Visa'
          }
        ],
        Shop: [
          {
            url: '#',
            text: 'Shop DC'
          },
          {
            url: '#',
            text: 'Shop DC Collectibles'
          }
        ],
        
      }
    }
}
</script>

<style scoped lang="scss">

  .footer-up {
    display: flex;
    background-image: url('../assets/img/footer-bg.jpg');

    .up {
      display: flex;

      .footer-link {
        display: flex;
        width: 30%;
        padding: 20px;
      }
    }

      .big-logo {
        width: 70%;
        position: relative;

        img {
          width: 400px;
          height: 400px;
          position: absolute;
          bottom: -55px;
          right: 30px;
        }
      }
    }  
  

  .social-section {
      background-color: #303030;
      height: 100px;
      display: flex;
      align-items: center;
      position: absolute;
      width: 100%;
      z-index: 998;

      .container90 {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .subscribe {
            border: 2px solid #0282F9;
            height: 40px;
            padding: 10px;

            a {
              color: white;
            }
          }

        .social-icon {
          display: flex;
          align-items: center;

          .follow {
            margin-right: 15px;

            a {
              color: #0282F9;
            }
          }

          ul {
            display: flex;

            li {
              margin: 0 5px;
            }
          }


        }
      }

      
  }

</style>