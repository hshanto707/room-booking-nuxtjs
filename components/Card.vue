<template>
  <NuxtLink :to="`/rooms/${card.id}`" class="card">
    <img :src="card.image" alt="">
    <h3>{{ card.title }}</h3>
    <p>{{ card.snippet.slice(0, 100) }}...</p>
  </NuxtLink>
</template>

<script>
  export default {
    props: ['card']
  }
</script>

<style lang="scss" scoped>
  .card {
    width: 100%;
    height: auto;
    border: none;
    overflow: hidden;
    padding: 10px;
    border: 2px solid white;
    border-radius: 0.5rem;
    text-decoration: none;
    transition: 0.5s;

    img {
      width: 100%;
      height: 250px;
      border-radius: 0.5rem;
    }
    h3 {
      font-size: 1.15rem;
      margin-top: 0.4rem;
      color: #212121
    }
    p {
      color: grey;
      bottom: 0;
    }
  }

  .card:hover {
    border: 2px solid gray;
  }
</style>