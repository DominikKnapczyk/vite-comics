<script>
export default {};
</script>

<template>
  <footer>
    <!-- FOOTER TOP -->
    <div class="footer-top">
      <div class="footer-top-container">
        <div class="footer-top-icon">
          <img src="/buy-comics-digital-comics.png" alt="digital-comics">
          <span>DIGITAL COMICS</span>
        </div>
        <div class="footer-top-icon">
          <img src="/buy-comics-merchandise.png" alt="digital-comics">
          <span>DC MERCHANDISE</span>
        </div>
        <div class="footer-top-icon">
          <img src="/buy-comics-subscriptions.png" alt="digital-comics">
          <span>SUBSCRIPTION</span>
        </div>
        <div class="footer-top-icon">
          <img src="/buy-comics-shop-locator.png" alt="digital-comics">
          <span>COMIC SHOP LOCATOR</span>
        </div>
        <div class="footer-top-icon">
          <img src="/buy-dc-power-visa.svg" alt="digital-comics">
          <span>DC POWER VISA</span>
        </div>
      </div>
    </div>

    <!-- FOOTER MIDDLE -->
    <div class="footer-middle">
      <div class="footer-middle-container">
        <div class="footer-middle-content">

          <!-- COLUMN 1 -->
          <div class="footer-middle-content-column">
            <h3>DC COMICS</h3>
            <a href="#">Characters</a>
            <a href="#">Comics</a>
            <a href="#">Movies</a>
            <a href="#">Tv</a>
            <a href="#">Games</a>
            <a href="#">Videos</a>
            <a href="#">News</a>

            <h3>SHOP</h3>
            <a href="#">Shop DC</a>
            <a href="#">Shop DC Collectibles</a>
          </div>

          <!-- COLUMN 2 -->
          <div class="footer-middle-content-column">
            <h3>DC</h3>
            <a href="#">Terms Of Use</a>
            <a href="#">Privacy policy (New)</a>
            <a href="#">Ad Choices</a>
            <a href="#">Advertising</a>
            <a href="#">Jobs</a>
            <a href="#">Subscriptions</a>
            <a href="#">Talent Workshop</a>
            <a href="#">CPSC Certificates</a>
            <a href="#">Ratings</a>
            <a href="#">Shop Help</a>
            <a href="#">Contact Us</a>
          </div>

          <!-- COLUMN 3 -->
          <div class="footer-middle-content-column">
            <h3>SITES</h3>
            <a href="#">DC</a>
            <a href="#">MAD Magazine</a>
            <a href="#">DC Kids</a>
            <a href="#">DC Universe</a>
            <a href="#">DC Power Visa</a>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="footer-bottom-container">
        <div class="footer-bottom-left">
          <button>SING-UP NOW!</button>
        </div>
        <div class="footer-bottom-right">
          <h3>FOLLOW US</h3>
          <img src="/footer-facebook.png" alt="digital-comics">
          <img src="/footer-twitter.png" alt="digital-comics">
          <img src="/footer-youtube.png" alt="digital-comics">
          <img src="/footer-pinterest.png" alt="digital-comics">
          <img src="/footer-facebook.png" alt="digital-comics">
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>

// FOOTER TOP
.footer-top {
  background-color: #0282F9;
  height: 220px;
  display: flex;
  justify-content: center;
  align-items: center;

    .footer-top-container {
    display: flex;
    justify-content: space-around;
    align-items: center;

    min-width: 1100px;
    width: 80vw;
    max-width: 1400px;

    .footer-top-icon {
      width: calc(100%/5);
      display: flex;
      align-items: center;
      cursor: pointer;
      padding-right: 15px;

      img {
        height: 50px;
        max-width: 50px;
        margin-right: 5px;
      }

      span {
        color: white;
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        font-size: 18px;
      }
    }
  }
}

// FOOTER MIDDLE
.footer-middle {
  display: flex;
  justify-content: center;
  align-items: center;

  height: 500px;
  background-image: url("/footer-bg.jpg");
  background-size: cover; 
  background-repeat: no-repeat;

  .footer-middle-container{
    display: flex;
    align-items: center;

    background-image: url("/dc-logo-bg.png");
    
    background-repeat: no-repeat;
    background-position: right;
    

    min-width: 1100px;
    width: 80vw;
    max-width: 1400px;
    height: 500px;

    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;

    .footer-middle-content {
      display: flex;

      .footer-middle-content-column {
        width: 200px;

        h3{
          color: white;
          font-size: 26px;
        }

        a {
          display: block;
          text-decoration: none;
          color: #959595;
          padding: 2px 0;
        }
      }
    }
  }
}

// FOOTER BOTTOM
.footer-bottom {
  display: flex;
  justify-content: center;
  align-items: center;

  height: 120px;
  background-color: #303030;

  .footer-bottom-container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    min-width: 1100px;
    width: 80vw;
    max-width: 1400px;

    .footer-bottom-left {

      button {
        padding: 13px 16px;
        color: white;
        font-size: 16px;
        font-weight: bold;
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        background-color: transparent;
        border: 2px solid #0282F9;
        cursor: pointer;
        transition: 1s;

        &:hover {
          background-color: #0282F9;
        }
      }
    }

    .footer-bottom-right {
      display: flex;
      align-items: center;

      h3{
          color: #0282F9;
          font-size: 20px;
          font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
          margin-right: 20px;
        }

      img {
        height: 32px;
        margin: 0 8px;
        cursor: pointer;
      }
    }
  }
}

</style>