<template>
  <div>
  {{dates}}
      <v-date-picker
        v-model="dates"
        multiple
      ></v-date-picker>
  </div>
</template>

<script>
  export default {
    data: () => ({
      dates: [],
    }),
  }
</script>

<style lang="scss" scoped>

</style>