<template>
  <main>
    <div class="contents">
      <div class="container90">
        <div class="content">
          Contents goes here
        </div>
      </div>
    </div>

    <div class="bonus">
      <div class="container90">
        <div class="card-container">
          <ul>
            <li v-for="(card, index) in cards" :key="index">
              <img :src="card.img" :alt="card.text">
              <h5>{{card.text}}</h5>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
    name: 'MyMain',
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
    height: 100px;
    background-color: black;
    color: white;
    display: flex;
    align-items: center;

    .content {
    color: white;
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

        img {
          width: 40px;
        }
      }
    }
  }
  
</style>