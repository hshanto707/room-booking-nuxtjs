<template>
  <div class="review-card mt-4">
    <div>
      <img :src="review.picture.large" alt="" />
    </div>
    <div class="text-container">
      <h4>{{ review.name.first }} {{ review.name.last }}</h4>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repellendus
        quam magni beatae possimus debitis.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["review"],
};
</script>

<style lang="scss" scoped>
.review-card {
  display: flex;

  img {
    width: 50px;
    height: 50px;
    border-radius: 100%;
  }
  
  .text-container {
    margin-left: 2rem;
  }

  p {
    color: grey;
  }
}
</style>
