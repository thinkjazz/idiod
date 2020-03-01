<template>
  <div>
    <Header />
    <main class="main-content">
      <nuxt />
    </main>
  </div>
</template>
<script>
import Header from '@/components/Header/Header'
export default {
  components: {
    Header
  }
}
</script>
<style>
* {
  box-sizing: border-box;
}
body {
  font-family: 'Source Sans Pro', Arial, sans-serif;
}
 .main-content {
   margin-top: 4.5rem;
 }
</style>
