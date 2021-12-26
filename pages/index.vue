<template>
  <div>
    <Hero />
    <DisplayCards
      v-for="cardInfo in cardInfos"
      :key="cardInfo.id"
      :cardSection="cardInfo"
    />
  </div>
</template>

<script>
  import { CardSections } from "@/assets/data.js"
  export default {
    data() {
      return {
        cardInfos: CardSections
      }
    }
  }
</script>
