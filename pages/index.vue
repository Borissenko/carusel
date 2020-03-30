<template>
  <div class="cont bb">
    <div v-swiper:mySwiper="opts">
      <div class="swiper-wrapper">
        <div class=" swiper-slide">
          Каждый для нас — 1
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 2
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 3
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 4
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 5
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 6
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 7
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 8
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 9
        </div>
        <div class=" swiper-slide">
          Каждый для нас — 1
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 2
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 3
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 4
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 5
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 6
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 7
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 8
        </div>
        <div class=" swiper-slide ">
          Каждый для нас — 9
        </div>
        <div class="swiper-button-prev" slot="button-prev"></div>
        <div class="swiper-button-next" slot="button-next"></div>
      </div>
    </div>
  </div>
</template>
<script>
  // import { mapGetters } from 'vuex'
  export default {
    data: () => ({
      opts: {
        slidesPerView: 'auto',
        spaceBetween: 10,
        initialSlide: 7,
        grabCursor: true,
        breakpoints: {   // like @media
          900: {
            slidesOffsetBefore: 24,
            slidesOffsetAfter: 24,
            spaceBetween: 24,
            grabCursor: false
          }
        }
      }
    })
  }
</script>

<style scoped>
  .cont {
    width: 600px;
    height: 300px;
    margin: 50px auto 0;
    border: orange 1px solid;
  }

  /*стационарный внешний контейнер*/
  /* автоматичекси добавляемые классы to v-swiper:
  swiper-container
  swiper-container-initialized
  swiper-container-horizontal"
  */
  .swiper-container {
    width: 100%; /* 100%- по умолчанию */
    height: 200px; /* auto- по умолчанию. Надо прописывать самому(!) */
    border: #a8a8a8 3px solid;
  }

  /*функция непонятна*/
  .swiper-container-initialized {
    background-color: #5b3ed8;
  }
  /*функция непонятна*/
  .swiper-container-horizontal {
    background-color: #d8093e;
  }

  /*слайдер-контейнер*/
  .swiper-wrapper {
    display: flex !important;
    width: fit-content; /* дб оч большим, чтобы вобрать все карточки, не auto. Auto- ширина будет как у swiper-container'a*/
    height: max-content; /* auto- по умолчанию, и это- достаточно */
    overflow: visible; /*лучше сделать visible*/
    border: #DD3D3D 1px dashed;
  }

  /*ОБЯЗАТЕЛЬНЫЙ(!) спец класс для отдельного слайда*/
  /*автоматичекси добавляемые классы к слайду:
  swiper-slide - но его прописывать надо явно, что бы задать свои стили,
  swiper-slide-active*/
  .swiper-slide {
    width: 160px; /*ширина слайда */
    height: 100px; /*высота слайда */
    background: #a3deff;
  }

  /*стиль слайда, который находиться в начале .swiper-container'a */
  .swiper-slide-active {
    background-color: #fc5c65;
  }
  /*стиль слайда, который находиться перед active-слайдом */
  .swiper-slide-prev{
    background-color: #fcf738;
  }
  /*стиль слайда, который находиться правее active-слайда */
  .swiper-slide-next{
    background-color: #46fc4b;
  }

  .cc {
    outline: red 1px solid;
  }

  .vv {
    outline: #2b9871 1px dashed;
  }

</style>
