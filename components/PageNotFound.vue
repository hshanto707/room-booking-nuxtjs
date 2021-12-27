<template>
  <div>
    <h1>Page Not Found!</h1>
    <img src="https://thumbs.dreamstime.com/b/sad-emoji-crying-vector-emoticon-isolated-white-background-214295176.jpg" alt="">
    <NuxtLink to="/"> Back To Home </NuxtLink>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
  div {
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    height: 90vh;
    margin: auto 0;

    h1 {
      font-size: 60px;
    }

    img {
      width: 20%;
      margin: 0 auto;
    }
  }
</style>