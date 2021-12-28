<template>
  <div class="item-container">
    <img :src="item.image" alt="" />
    <div class="text-container">
      <h4>{{ item.title }}</h4>
      <p>{{ item.description }}</p>
      <h5>Booked Date:</h5>
      <p v-for="date in item.bookingDates" :key="date">{{date}}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["item"],
};
</script>

<style lang="scss" scoped>
.item-container {
  display: flex;
  margin: 3rem 0; 
  
  .text-container {
    padding: 0 1rem;
  }

  img {
    width: 200px;
    border-radius: 0.5rem;
    height: 11rem;
  }
  
  p {
    font-size: 0.8rem;
    color: grey;
  }
}
</style>
