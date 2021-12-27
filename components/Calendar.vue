<template>
  <div>
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
      menu: false,
    }),
  }
</script>

<style lang="scss" scoped>

</style>