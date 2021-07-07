// ------------------------------------------------HTML------------------------------------------------------------
<template>
  <div class="container-main">

    <div class="jumbotron">
      <img src="img/jumbotron.jpg" alt="">
    </div>

    <div class="container-fumetti">
      <button>CURRENT SERIES</button>
      <ul class="first-row">
        <li v-for="(fumetto, index) in fumetti" :key="index">
          <img :src="fumetto.url" alt="fumetto">
          <p> {{ fumetto.series }} </p>
        </li>
      </ul>
      <br>
      <ul class="second-row">
        <li v-for="(fumetto2, index) in fumetti2" :key="index">
          <img :src="fumetto2.url" alt="fumetto">
          <p> {{ fumetto2.series }} </p>
        </li>
      </ul>
      <button class="btn">LOAD MORE</button>
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



// ------------------------------------------------JAVASCRIPT----------------------------------------------------
<script>
import arrayCards from '@/data/arrayCards';
import arrayFumetti from '@/data/arrayFumetti';
import arrayFumetti2 from '@/data/arrayFumetti2';

export default {
  name: 'Main',
  data() {
    return {
      cards: arrayCards,
      fumetti: arrayFumetti,
      fumetti2: arrayFumetti2
    }
  }
}
</script>



// -------------------------------------------------------CSS----------------------------------------------------
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

  .jumbotron img{
    display: block;
    height: 800px;
    width: 100%;
  }

  .container-fumetti {
    background-color: rgb(22, 22, 22);
    display: flex;
    height: 800px;
    color: white;
    text-transform: uppercase;
    font-size: 12px;
    overflow: hidden;
    width: 100%;
    flex-wrap: wrap;
  }

  .container-fumetti img {
    width: 200px;
    height: 200px;
    margin-bottom: 10px;
  }

  .container-fumetti li {
    width: 270px;
    margin: 10px;
  }

  .first-row {
    margin-top: 50px;
    margin-bottom: 100px;
    margin-left: 30px;
  }

  .second-row {
    margin-top: 50px;
    margin-left: 30px;
    margin-bottom: 100px;
  }

  .btn {
    width: 150px;
    height: 30px;
    position: relative;
    left: 45%;
    top: 30px;
    margin-top: 45px;
    margin: 25px;
    font-size: 18px;
    padding: 3px;
  }

  button {
    color: white;
    background-color: rgb(0, 132, 255);
    cursor: pointer;
    font-weight: 800;
    font-size: 21px;
    position: absolute;
    padding: 15px;
    top: 776px;
    left: 15%;
  }
</style>
