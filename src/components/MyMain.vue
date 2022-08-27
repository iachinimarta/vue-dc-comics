<template>
  <main>
    <div class="contents">
        <div class="content">
          <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="">
          </div>
          <div class="current-series">CURRENT SERIES</div>
          <MyCards/>
          <div class="d-flex">
            <div class="load-more">
              <a href="#">
                LOAD MORE
              </a>
            </div>
          </div>
          
        </div>
    </div>

    <div class="bonus">
      <div class="container90">
        <div class="card-container">
          <ul>
            <li v-for="(card, index) in cards" :key="index">
              <div class="img-container">
                <img :src="card.img" :alt="card.text">
              </div>
              <h5>
                <a href="#">
                  {{card.text}}
                </a>
              </h5>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import MyCards from './MyCards.vue';

export default {
    name: 'MyMain',
    components: {
      MyCards
    },
    data() {
      return {
        cards: [
          {
            img: require('../assets/img/buy-comics-digital-comics.png'),
            text: 'DIGITAL COMICS'
          },
          {
            img: require('../assets/img/buy-comics-merchandise.png'),
            text: 'DC MERCHANDISE'
          },
          {
            img: require('../assets/img/buy-comics-subscriptions.png'),
            text: 'SUBSCRIPTION'
          },
          {
            img: require('../assets/img/buy-comics-shop-locator.png'),
            text: 'COMIC SHOP LOCATOR'
          },
          {
            img: require('../assets/img/buy-dc-power-visa.svg'),
            text: 'DC POWER VISA'
          },

        ]
      }
    }
}
</script>

<style scoped lang="scss">

  .contents {
    background-color: black;
    color: white;
    display: flex;
    align-items: center;

    .content {
      color: white;
      width: 100%;

        .jumbotron {
          width: 100%;
          height: 300px;
          margin-top: 90px;
          

          img {
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: 0 0;
          }
        }

        .d-flex {
          display: flex;
          justify-content: center;
          margin-bottom: 50px;

          .load-more {
            background-color: #0282f9;
            width: 150px;
            height: 30px;
            line-height: 30px;
            text-align: center;
          }
        }

        .current-series {
            background-color: #0282F9;
            height: 40px;
            width: 200px;
            display: inline-block;
            padding: 10px;
            text-align: center;
            transform: translateX(50%);
        }
    }
    
  }

  .bonus {
    height: 100px;
    background-color: #0282F9;
    display: flex;
    align-items: center;

    ul {
      display: flex;
      justify-content: space-between;

      li {
        display: flex;
        align-items: center;

        .img-container {
          margin-right: 5px;
          width: 50px;
          height: 50px;

          img {
            width: 100%;
            height: 100%;
            object-fit: contain;
          }
        }

        h5 {
          font-size: 10px;
          font-weight: normal;
          
          a {
            color: white;
          }
        }
      }
    }
  }
  
</style>