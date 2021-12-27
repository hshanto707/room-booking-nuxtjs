<template>
  <div class="mb-12">
    <h1>{{ cardSection.title}}</h1>
    <p>{{ cardSection.snippet }}</p>
    <div class="cards-container">
      <Card
        v-for="card in cardSection.cards"
        :key="card.id"
        :card="card"
      />
    </div>
  </div>
</template>

<script>
  export default {
    props: ['cardSection']
  }
</script>

<style lang="scss" scoped>
  .cards-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
  }
</style>