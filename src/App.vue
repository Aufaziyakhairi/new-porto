<template>
  <header class="w-full h-[100vh]">
    <transition enter-active-class="transition transform duration-5000 ease-out" enter-from-class="opacity-0"
      enter-to-class="opacity-100">
      <div v-if="show"
        class="bottom-0 left-0 duration-700 absolute border-[1px] w-[500px] h-[200px] align-text-bottom pt-[50px] bg-white z-[100]">
        <h1 class=" text-5xl font-bold">
          Welcome</h1>
        <p class="text-2xl">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugit, fuga.</p>
      </div>
    </transition>
    <img src="./assets/Logo.svg" alt="Logo" class="w-[48%]  mx-auto mt-[100px]" />
    <div class=" absolute top-[100px] left-[100px] w-[25%] border-[1px] p-[20px] bg-white z-[100] text-left">
      <h1 class="text-2xl font-bold">Website</h1>
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugit, repellat.</p>
    </div>
    <div
      class=" z-[-100] absolute left-[200px] top-[300px] w-[900px] border-black border-[100px] rotate-[30deg] rounded-full">
    </div>
    <div
      class=" z-[-100] absolute left-[250px] top-[300px] w-[800px] border-black border-[100px] rotate-[-30deg] rounded-full">
    </div>
    <div
      class=" z-[-100] absolute left-[300px] top-[300px] w-[700px] border-black border-[100px] rotate-[0deg] rounded-full">
    </div>
    <div
      class=" z-[-100] absolute left-[350px] top-[300px] w-[600px] border-black border-[100px] rotate-[90deg] rounded-full">
    </div>
    <div class=" absolute bottom-[100px] right-[100px] w-[25%] border-[1px] p-[20px] bg-white z-[100] text-right a">
      <h1 class="text-2xl font-bold">Developer</h1>
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugit, repellat.</p>
    </div>
    <a href="" class="z-[100]">
      <i
        class="fas fa-chevron-down absolute left-[50%] text-3xl bottom-0 animate-bounce duration-700 hover:text-gray-400"></i>
    </a>
  </header>
  <NavigationBar />
  <main>
    <section class="w-full h-[100vh]">
      <Swiper class=" w-full h-[100vh] mySwiper" :modules="modules" :direction="'vertical'" :autoplay="{ delay: 1500 }"
        :pagination="{ clickable: true, dynamicBullets: true }" :loop="true">
        <SwiperSlide class="w-full h-[100vh] relative overflow-clip">
          <img src="./assets/Logo.svg" alt="" class="w-full">
          <div
            class=" flex flex-wrap justify-around items-center absolute bottom-0 left-0 w-[50%] bg-white z-[100] border-[1px] p-[1px]">
            <h1 class="text-center text-5xl font-bold w-full">Name Project</h1>
            <p class="w-full text-justify text-3xl">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Possimus,
              exercitationem.</p>
            <a href="" class="text-right text-2xl hover:bg-black hover:text-white duration-700 p-[10px]">Let's Go</a>
          </div>
        </SwiperSlide>
        <SwiperSlide class="w-full h-[100vh] relative overflow-clip">
          <img src="./assets/Logo.svg" alt="" class="w-full">
          <div
            class=" flex flex-wrap justify-around items-center absolute bottom-0 left-0 w-[50%] bg-white z-[100] border-[1px] p-[1px]">
            <h1 class="text-center text-5xl font-bold w-full">Name Project</h1>
            <p class="w-full text-justify text-3xl">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Possimus,
              exercitationem.</p>
            <a href="" class="text-right text-2xl hover:bg-black hover:text-white duration-700 p-[10px]">Let's Go</a>
          </div>
        </SwiperSlide>
      </Swiper>
    </section>
    <section class="w-full h-[100vh] grid">
      <div class=" col-start-1 col-end-1 row-start-1 row-end-1">
        <img src="./assets/Logo.svg" alt="">
      </div>
      <div class=" col-start-2 col-end-3">
        <h1>About Me</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est itaque repudiandae unde rem ratione obcaecati
          voluptatum impedit necessitatibus, optio nihil asperiores, natus, doloribus quo expedita cum recusandae
          deserunt perspiciatis eaque.</p>
      </div>
      <div>
        <h1>I Can</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti deserunt maiores optio magni, perferendis
          iure sunt? Ad, fuga consectetur mollitia iusto omnis neque delectus sint, eum pariatur, vero nihil iure.</p>
      </div>
      <div>
        <i></i>
        <i></i>
        <i></i>
        <i></i>
        <i></i>
        <i></i>
      </div>
    </section>
  </main>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import NavigationBar from './components/NavigationBar.vue';
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/pagination';
import { Autoplay, Pagination } from 'swiper/modules';

const modules = [Pagination, Autoplay,];
const show = ref(false);


onMounted(() => {
  show.value = true; // Elemen akan muncul otomatis setelah halaman dimuat
});
</script>

<style scoped></style>
