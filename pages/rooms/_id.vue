<template>
  <div v-if="room" class="container my-5">
    <div class="hero-container mt-4 mb-8">
      <img :src="room.image" alt="" />
      <div class="room-info">
        <h1>{{ room.title }}</h1>
        <p class="snippet">{{ room.snippet }}</p>

        <!-- CALENDAR -->

        <v-date-picker v-model="dates" multiple></v-date-picker>

        <v-btn @click="addItem({id: room.id, dates: dates})" color="primary">Rent</v-btn>
      </div>
    </div>
    <hr />
    <div class="whats-included-container mt-8">
      <div class="included-container">
        <h4>Super Effective</h4>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores,
          dolorem.
        </p>
      </div>
      <div class="included-container">
        <h4>Clean & Tidy</h4>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores,
          dolorem.
        </p>
      </div>
      <div class="included-container">
        <h4>Cancel Anytime</h4>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores,
          dolorem.
        </p>
      </div>
      <div class="included-container">
        <h4>Satisfaction Guaranteed</h4>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores,
          dolorem.
        </p>
      </div>
    </div>
    <div class="description-container mb-8">
      <p>
        {{ room.description }}
      </p>
    </div>
    <hr />
    <Reviews />
  </div>
  <div v-else class="container padding">
    <PageNotFound />
  </div>
</template>

<script>
import { mapMutations } from "vuex";
import { mapGetters } from "vuex";
export default {
    data: () => ({
      dates: [],
    }),
  computed: {
    room() {
      return this.$store.getters.getRoomById(this.$route.params.id);
    },
  },
  methods: {
    ...mapMutations(["addItem"]),
  },
};
</script>

<style lang="scss" scoped>
.hero-container {
  display: flex;
  justify-content: space-between;
  gap: 0 20px;

  img {
    width: 50%;
    border-radius: 10px;
  }
}
</style>
