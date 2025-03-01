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
    <section class="w-full h-[100vh] flex flex-wrap items-center p-[100px] relative ">
      <div class=" col-start-1 col-end-1 row-start-1 row-end-1 w-[30%] border-[1px] p-[50px] skew-y-[10deg] h-[44%] bg-gray-300">
        <img src="./assets/Logo.svg" alt="" class="w-[50%] mx-auto">
      </div>
      <div class=" col-start-2 col-end-3 w-[70%] border-[1px] p-[55px] skew-y-[-4deg] h-[44%] shadow-2xl bg-white">
        <h1 class="text-5xl font-bold">About Me</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est itaque repudiandae unde rem ratione obcaecati
          voluptatum impedit necessitatibus, optio nihil asperiores, natus, doloribus quo expedita cum recusandae
          deserunt perspiciatis eaque.</p>
      </div>
      <div class="w-[70%] border-[1px] p-[65px] skew-y-[4deg] bg-gray-300 h-[44%]">
        <h1 class="text-5xl font-bold">I Can</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti deserunt maiores optio magni, perferendis
          iure sunt? Ad, fuga consectetur mollitia iusto omnis neque delectus sint, eum pariatur, vero nihil iure.</p>
      </div>
      <div class=" bg-white w-[30%] border-[1px] p-[10px] flex flex-wrap justify-around items-center h-[44%] transform skew-y-[-10deg] shadow-2xl">
        <i class="fas fa-brands fa-sass text-3xl"></i>
        <i class="fas fa-brands fa-sass text-3xl"></i>
        <i class="fas fa-brands fa-sass text-3xl"></i>
        <i class="fas fa-brands fa-sass text-3xl"></i>
        <i class="fas fa-brands fa-sass text-3xl"></i>
        <i class="fas fa-brands fa-sass text-3xl"></i>
      </div>
      <span class=" absolute border-[1px] h-[100px] w-[1000px] top-0 left-0 z-[-100]"></span>
      <span class=" absolute border-[1px] h-[500px] w-[100px] bottom-0 left-0 z-[-100]"></span>
      <span class=" absolute border-[1px] h-[500px] w-[100px] top-0 right-0 z-[-100]"></span>
      <span class=" absolute border-[1px] h-[100px] w-[1000px] bottom-0 right-0 z-[-100]"></span>
    </section>
    <section class="w-full h-[100vh] flex flex-wrap items-center p-[100px]">
      <h1 class="text-5xl font-bold text-center w-full">Contact</h1>
      <form action="" class="grid w-[50%] mx-auto gap-[10px]">
        <input type="text" placeholder="Name" class=" col-start-1 col-end-1 row-start-1 row-end-1 p-[10px] border-[1px]">
        <input type="email" placeholder="Email" class=" p-[10px] border-[1px] col-start-1 col-end-1 row-start-2 row-end-2">
        <textarea name="" id="" cols="30" rows="10" placeholder="Message"
          class=" p-[10px] border-[1px] col-start-2 col-end-2 row-start-1 row-end-3"></textarea>
        <button class="w-[100%] p-[10px] bg-black text-white col-start-1 col-end-3 mx-auto hover:bg-white hover:text-black border-[1px] duration-700">Send</button>
      </form>
    </section>
  </main>
  <footer class="w-full bg-black text-white text-center p-[100px] flex flex-wrap items-center gap-[50px] relative">
    <h1 class="text-5xl font-bold w-full">Thank You</h1>
    <ul class="flex flex-wrap gap-[10px] list-none items-center text-center w-full justify-center">
      <li class="text-3xl"><a href=""><i class="fas fa-brands fa-instagram"></i>Instagram</a></li>
      <li class="text-3xl"><a href=""><i class="fas fa-brands fa-github"></i>Github</a></li>
    </ul>
    <span class="absolute w-[1000px] h-[50px] bg-white top-0 left-0"></span>
    <span class="absolute w-[1000px] h-[50px] bg-white bottom-0 right-0"></span>
    <i class="fas fa-star text-2xl absolute right-[10px]"></i>
    <i class="fas fa-star text-3xl absolute right-[50px] top-[100px]"></i>
    <i class="fas fa-star text-4xl absolute right-[80px] top-[50px]"></i>
    <i class="fas fa-star text-2xl absolute right-[150px]"></i>
    <i class="fas fa-star text-3xl absolute right-[120px] top-[100px]"></i>
    <i class="fas fa-star text-2xl absolute left-[10px]"></i>
    <i class="fas fa-star text-3xl absolute left-[50px] top-[100px]"></i>
    <i class="fas fa-star text-4xl absolute left-[80px] top-[50px]"></i>
    <i class="fas fa-star text-2xl absolute left-[150px]"></i>
    <i class="fas fa-star text-3xl absolute left-[120px] top-[100px]"></i>
  </footer>
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
