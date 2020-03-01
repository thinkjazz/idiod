<template>
  <header class="main-header">
    <nav class="main-nav">
      <ul class ="nav-links">
        <nuxt-link  to ="/" class="nav-link"  tag="li">
        <a>Все посты</a>
        </nuxt-link>
        <nuxt-link  to = "/about" class="nav-link" tag="li">
        <a>Об идиодах</a>
      </nuxt-link>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
  .main-header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background: #222f3e;
    height: 4.5rem;
  }
  .main-nav {
    height: 100%;
  }
  .nav-links {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
  }
  .nav-link.nuxt-link-exact-active {
    border-bottom: 3px solid #feca57;
  }
  .nav-link {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 1rem;
    padding: 0.3rem;
  }
  .nav-link a {
    font-weight: 600;
    display: block;
    text-decoration: none;
    color: #feca57;
  }
  .nav-link a:hover, .nav-link a:active, .nav-link.nuxt-link-exact-active a{
  color:#c8d6e5;
  }
</style>
