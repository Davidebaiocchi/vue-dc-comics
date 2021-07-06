<template>
  <div class="container">
    <img src="img/dc-logo.png" alt="Logo Dc">
    <ul> 
      <li v-for="(link, index) in links" :key="index"><a href="link.url" :class="{ active: link.current }"> {{ link.text }} </a></li>
    </ul>
  </div>
</template>


<script>
export default {
  name: 'Header',
  data() {
    return {
      links: [
        {
          text: 'characters',
          url: '#',
          current: true
        },
        {
          text: 'comics',
          url: '#',
          current: false
        },
        {
          text: 'movies',
          url: '#',
          current: false
        },
        {
          text: 'tv',
          url: '#',
          current: false
        },
        {
          text: 'games',
          url: '#',
          current: false
        },
        {
          text: 'collectibles',
          url: '#',
          current: false
        },
        {
          text: 'videos',
          url: '#',
          current: false
        },
        {
          text: 'fans',
          url: '#',
          current: false
        },
        {
          text: 'news',
          url: '#',
          current: false
        },
        {
          text: 'shop',
          url: '#',
          current: false
        },
      ]
    }
  }
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
    height: 120px;
  }

  li:active {
    border-bottom: 5px solid rgb(0, 132, 255);
  }

  a {
    text-transform: uppercase;
    padding: 0 15px;
    cursor: pointer;
    font-weight: 600;
    color: rgb(75, 75, 75);
    text-decoration: none;
  }

  a:hover {
    color: rgb(0, 132, 255);
  }
</style>
