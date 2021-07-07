<template>
  <div class="container">
    <div class="upper">
      <div class="left-upper-section">
        
      </div>

      <div class="right-upper-section">
        
      </div>
    </div>

    <div class="bottom">
      <div class="social">
        <button>SIGN-UP NOW!</button>
        <span class="follow">FOLLOW US</span>
        <span>
          <img src="img/per.png" alt="periscope">
          <img src="img/pinterest.png" alt="">
          <img src="img/fb.png" alt="">
          <img src="img/twitter.png" alt="">
          <img src="img/yt.png" alt="">
        </span>
      </div>
    </div>
  </div>
</template>






<script>
export default {
  name: 'Footer',
}
</script>





<style lang="scss" scoped>
@import '@/style/vars.scss';
/* parte superiore footer */
.upper {
  background-image: url(../assets/footer-bg.jpg);
  height: 400px;
  background-size: cover;
}

  .right-upper-section{
    background-image: url(../assets/dc-logo-bg.png);
    height: 100%;
    background-repeat: no-repeat;
    margin-left: 60%;
  }


/* parte inferiore footer */
  .bottom {
    height: 100px;
    background-color: rgb(44, 44, 44);
    color: $blue;
    font-weight: 800;
    padding-top: 35px;
    z-index: 1;
  }

  img {
    margin: 5px;
  }

  .follow:hover {
    color: red;
    cursor: pointer;
  }

  .follow {
    position: relative;
    bottom: 15px;
    margin-right: 10px;
  }

  button {
    background-color: transparent;
    border: 3px solid $blue;
    color: white;
    font-weight: 800;
    font-size: 22px;
    padding: 10px;
    margin-left: 10%;
    margin-right: 50%;
    position: relative;
    bottom: 15px;
  }
</style>
