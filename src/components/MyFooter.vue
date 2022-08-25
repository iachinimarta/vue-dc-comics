<template>
  <footer>
    <div class="footer-up">
      <div class="container90 up">
        <div class="footer-link">
          <ul>
            <div><a href="#">DC COMICS</a></div>
            <li><a href="#">Link del footer</a></li>
          </ul>
          <ul>
            <div><a href="#">DC</a></div>
            <li><a href="#">Link del footer</a></li>
          </ul>
          <ul>
            <div><a href="#">SITES</a></div>
            <li><a href="#">Link del footer</a></li>
          </ul>
          <ul>
            <div><a href="#">SHOP</a></div>
            <li><a href="#">Link del footer</a></li>
          </ul>
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
          <div><a href="#">FOLLOW US</a></div>
          <ul>
            <li><a href="#">Icone</a></li>
          </ul>
        </div>
      </div>
      
    </div>

  </footer>
</template>

<script>
export default {
    name: 'MyFooter'
}
</script>

<style lang="scss">

  .footer-up {
    display: flex;
    background-image: url('../assets/img/footer-bg.jpg');

    .up {
      display: flex;

      .footer-link {
        display: flex;
        width: 30%;
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

        .social-icon {
          display: flex;
        }
      }
  } 

</style>