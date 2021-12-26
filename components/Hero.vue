<template>
  <div class="container mb-12">
    <div class="hero">
      <div class="hero-info">
        <h1 class="header">Find The Best Comfortable Room In The City</h1>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Alias
          facilis soluta unde voluptas illo repellat nihil veritatis cumque
          fuga, consectetur quisquam. Reprehenderit illum rerum eius blanditiis?
          Dicta temporibus repellat nulla.
        </p>
        <v-btn color="primary">Explore Rooms</v-btn>
      </div>
      <div>
        <img
          src="https://media.istockphoto.com/vectors/people-arrive-to-hotel-men-and-women-with-baggage-vector-illustration-vector-id1226006801?b=1&k=20&m=1226006801&s=612x612&w=0&h=BCDa_CvmEstUqoxqwlr1XdDh1YebJy-3rZIDyO_UJUs="
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.hero {
  display: grid;
  grid-template-columns: repeat(2, 1fr);

  .hero-info {
    margin: auto 0;

    h1 {
      font-size: 40px;
      font-weight: 900;
    }
  }

  img {
    width: 100%;
  }
}
</style>
