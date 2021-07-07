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


<style lang="scss" scoped>
@import '@/style/vars.scss';
  .container {
    height: 120px;
    line-height: 120px;
    position: fixed;
    display: flex;
    background-color: white;
    width: 100%;
    z-index: 1;
  }

  img {
    height: 100%;
    padding: 10px 0;
    margin-left: 300px;
    margin-right: 300px;
  }

  ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
  }

  li:active {
    border-bottom: 5px solid $blue;
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
    color: $blue;
  }
</style>
