<template>
  <div color="red" class="d-flex justify-space-between align-center">
    <NuxtLink to="/" class="logo">Find Room</NuxtLink>
    <NuxtLink to="/my-bookings" class="my-bookings">My Bookings</NuxtLink>

  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');

  .logo {
    font-family: 'Lobster';
    font-size: 40px;
    text-decoration: none;
    color: #212121;
  }

  .my-bookings {
    margin-left: auto;
    color: #212121;
  }
</style>