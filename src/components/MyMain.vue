<template>
  <main>
    <div class="contents">
        <div class="content">
          <MyCards/>
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
      height: 100%;
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