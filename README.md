# nuxt_carusel для мобильника
1. В package.json прописываем "vue-awesome-swiper": "^3.1.3", именно версию 3.1.3(!).
2. инстиллируем ее by yarn install
=>> в папке node_modules появится vue-awesome-swiper/dist/ssr

Для подстраховки файлы из node_modules/vue-awesome-swiper сохранил в папке плагинов

3. прописываем рлагин vue-awesome-swiper
import Vue from 'vue'
import VueAwesomeSwiper from 'vue-awesome-swiper/dist/ssr'

Vue.use(VueAwesomeSwiper)

 и регистрируем его в nuxt.config.js
  plugins: [
    { src: '~/plugins/vue-awesome-swiper', ssr: false }
  ],
4. код карусели- см. в файле.  
  
  
  
  
