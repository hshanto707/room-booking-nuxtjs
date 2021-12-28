<template>
  <div>
    <MyItem 
      v-for="myBooking in myBookings"
      :key="myBooking.id"
      :item="myBooking"
    />
  </div>
</template>

<script>
import { mapState } from 'vuex';

    export default {
        computed: {
            ...mapState([
                'myBookings'
            ])
        }
    }
</script>

<style lang="scss" scoped>

</style>