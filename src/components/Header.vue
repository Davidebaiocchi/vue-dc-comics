<template>
  <div class="container">
    <img src="@/assets/dc-logo.png" alt="Logo Dc">
    <ul> 
      <li>characters</li>
      <li>comics</li>
      <li>movies</li>
      <li>tv</li>
      <li>games</li>
      <li>collectibles</li>
      <li>videos</li>
      <li>fans</li>
      <li>news</li>
      <li>shop</li>
    </ul>
  </div>
</template>


<script>
export default {
  name: 'Header',
}
</script>


<style scoped>
  .container {
    height: 120px;
    line-height: 120px;
  }

  img {
    height: 100%;
    padding: 10px 0;
    margin-left: 300px;
  }

  ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
    position: absolute;
    top: 0;
    right: 250px;
  }

  li {
    text-transform: uppercase;
    padding: 0 15px;
    cursor: pointer;
    font-weight: 600;
    color: rgb(75, 75, 75);
  }

  li:hover {
    color: rgb(0, 132, 255);
  }
</style>
