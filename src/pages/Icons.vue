<template>
  <section class="py-5">
    <div class="container px-5 mb-5">
      <div class="text-center mb-5">
        <h1 class="display-5 fw-bolder mb-0">
          <span class="text-gradient d-inline">Picture Gallery</span>
        </h1>
      </div>
      <div class="row gx-5 justify-content-center">
        <div class="col-lg-11 col-xl-9 col-xxl-8">
          <div
            v-for="picture in pictureGallery"
            :key="picture.title"
            class="card overflow-hidden shadow rounded-4 border-0 mb-5"
          >
            <div class="card-body p-0">
              <div class="d-flex align-items-center">
                <div class="p-5">
                  <h2 class="fw-bolder">{{ picture.title }}</h2>
                  <p>{{ picture.description }}</p>
                </div>
                <img class="img-fluid uniform-img" :src="picture.image" :alt="picture.title" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      pictureGallery: [
        {
          title: "Pitch",
          description: "The OG of the house. Mama of all felines.",
          image: require('@/assets/img/cats/pitch.jpg'),
        },
        {
          title: "Patch",
          description: "The chunky king. Only boy, maximum loaf.",
          image: require('@/assets/img/cats/patch.jpg'),
        },
        {
          title: "Panda",
          description: "Nighttime opera star. Meow maestro.",
          image: require('@/assets/img/cats/panda.jpg'),
        },
        {
          title: "Riri",
          description: "My soul twin. Anti-social and pro-nap.",
          image: require('@/assets/img/cats/Riri.jpg'),
        },
        {
          title: "Selena",
          description: "The clingy baby. All the feels, all the time.",
          image: require('@/assets/img/cats/selena.jpg'),
        },
        {
          title: "Pepsi",
          description: "The zoomie champion. Small, fast, chaos.",
          image: require('@/assets/img/cats/pepsi.jpg'),
        },
      ],
    };
  },
};
</script>

<style>
.card-body {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.uniform-img {
  width: 250px;
  height: 250px;
  object-fit: cover;
  border-radius: 10px;
  margin-right: 15px;
}
</style>
