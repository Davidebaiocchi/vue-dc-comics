<template>
  <div class="container-main">
    <div class="container">
      <p> → → → Content goes here! ← ← ←  </p>
    </div>
    <div class="container-main-blue">
      <ul>
        <li v-for="(card, index) in cards" :key="index">
          <img :src="card.image" alt="">
          <span> {{ card.text }} </span>
        </li> 
      </ul>
    </div>
  </div>
</template>


<script>
export default {
  name: 'Main',
  data() {
    return {
      cards: [
        {
          image:'img/digital.png',
          text:'Digital Comics'
        },
        {
          image:'img/merch.png',
          text:'dc merchandise'
        },
        {
          image:'img/sub.png',
          text:'Sebscription'
        },
        {
          image:'img/shop.png',
          text:'Comic shop'
        },
        {
          image:'img/power.svg',
          text:'Dc power visa'
        },
      ]
    }
  }
}


</script>


<style scoped>
  .container {
    background-color: black;
    color: white;
    height: 120px;
    line-height: 120px;
    font-size: 40px;
    text-align: center;
  }
  .container-main-blue {
    background-color: rgb(0, 132, 255);
    height: 120px;
  }
  .container-main-blue img {
    height: 50px;
    vertical-align: -15px;
    margin-right: 10px;
  }

  ul {
    display: flex;
    justify-content: center;
    height: 120px;
    padding-top: 30px;
  }

  li {
    padding: 0 40px;
    cursor: pointer;
  }
  
  span {
    color: white;
    font-size: 20px;
    text-transform: uppercase;
  }
</style>
