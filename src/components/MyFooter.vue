<template>
  <footer>
    <div class="footer-up">
      <div class="container90 up">
        <div class="footer-link">

          <FooterMenu :title="'DC COMICS'" :urls="DcComics" :color="'white'"/>

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
        <div class="subscribe"><a href="#"> SIGN-UP NOW!</a></div>
        <div class="social-icon">
          <div class="follow">
            <a href="#">FOLLOW US</a>
          </div>
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
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          }
        ],
        DC: [
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          }
        ],
        Sites: [
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          }
        ],
        Shop: [
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
          },
          {
            url: '#',
            text: 'link'
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
        align-items: center;
      }
    }

      .big-logo {
        width: 70%;
        text-align: center;

        img {
          width: 300px;
          height: 300px;
        }
      }
    }  
  

  .social-section {
      background-color: #303030;
      height: 100px;
      display: flex;
      align-items: center;

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