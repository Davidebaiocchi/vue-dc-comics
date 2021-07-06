<template>
  <div class="container-main">
    <div class="container">
      <p> → → → Content goes here! ← ← ←  </p>
    </div>
    <div class="container-main-blue">
      <ul>
        <li>
          <img src="@/assets/digital.png" alt="assets">
          <span>Digital Comics</span>
        </li>
        <li>
          <img src="@/assets/merch.png" alt="assets">
          <span>Digital Comics</span>
        </li>
        <li>
          <img src="@/assets/sub.png" alt="assets">
          <span>Digital Comics</span>
        </li>
        <li>
          <img src="@/assets/shop.png" alt="assets">
          <span>Digital Comics</span>
        </li>
        <li>
          <img src="@/assets/pow.svg" alt="assets">
          <span>Digital Comics</span>
        </li>
      </ul>
    </div>
  </div>
</template>


<script>
export default {
  name: 'Main',
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
