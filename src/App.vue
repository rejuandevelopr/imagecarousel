<script setup>

const allimage=[
  {
    image:'https://i.ibb.co/Hx0WWdb/pexels-luis-del-r-o-15286.jpg',
    title:'image 1',
    alt:'Image 1',
    click:'Luis del'
  },

  {
    image:'https://i.ibb.co/gTZyyD2/pexels-quang-nguyen-vinh-2649403.jpg',
    title:'image 2',
    alt:'Image 1',
    click:'Quang nguyen'
  },

  {
    image:'https://i.ibb.co/QYWJNCn/pexels-brady-knoll-5409751.jpg',
    title:'image 3',
    alt:'Image 1',
    click:'Brady knoll'
  },

  {
    image:'https://i.ibb.co/gTZyyD2/pexels-quang-nguyen-vinh-2649403.jpg',
    title:'image 4',
    alt:'Image 1',
    click:'Quang'
  }


]


  

</script>

<template>
  <h1 class="mb-5 text-center"> Image Carousel </h1>
<div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3" aria-label="Slide 4"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active ">
      <img :src="allimage[0].image" :alt="allimage[0].alt" :title="allimage[0].title">
      <h2>Captured by {{ allimage[0].click }}</h2>
    </div>
    <div class="carousel-item">
      <img :src="allimage[1].image" :alt="allimage[1].alt" :title="allimage[1].title">
      <h2>Captured by {{ allimage[1].click }}</h2>
    </div>
    <div class="carousel-item">
      <img :src="allimage[2].image" :alt="allimage[2].alt" :title="allimage[2].title">
      <h2>Captured by {{ allimage[2].click }}</h2>
    </div>
    <div class="carousel-item">
      <img :src="allimage[3].image" :alt="allimage[3].alt" :title="allimage[3].title">
      <h2>Captured by {{ allimage[3].click }}</h2>
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>

</template>

<style scoped>
.carousel-indicators {
    bottom: 45px;
}




</style>
