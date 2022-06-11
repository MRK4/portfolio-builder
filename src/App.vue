<template>
  <div class="accent-cta bg-white dark:bg-darkmode_background p-16 flex flex-col justify-center items-center space-y-12 scroll-smooth">
    <div class="w-full flex flex-row justify-end">
      <div class="cursor-pointer p-2">
        <i class="toggle1 icon-light fa-regular fa-moon fa-lg text-cta fill-current drop-shadow" alt="îcone de lune"></i>
        <i class="toggle2 icon-dark fa-solid fa-sun fa-lg text-[#21243D] fill-current dark:text-yellow-500 drop-shadow hidden" alt="îcone de soleil"></i>
      </div>
    </div>
    <Portfolio_Header/>
    <div class="flex w-1/3 h-px bg-customblack dark:bg-customgray opacity-50"></div>
    <Portfolio_Grid_Showcase />
    <Portfolio_Footer />
  </div>
</template>

<script>
import Portfolio_Header from '@/components/Portfolio_Header.vue'
import Portfolio_Grid_Showcase from '@/components/Portfolio_Grid_Showcase.vue'
import Portfolio_Footer from '@/components/Portfolio_Footer.vue'

export default {
  name: 'App',
  components: {
    Portfolio_Header,
    Portfolio_Grid_Showcase,
    Portfolio_Footer
  },
  mounted: function () {
    this.$nextTick(function () {
      const toggle1 = document.querySelector('.toggle1');
      const toggle2 = document.querySelector('.toggle2');
      const html = document.querySelector('html');
      const iconLight = document.querySelector('.icon-light');
      const iconDark = document.querySelector('.icon-dark');
      toggle1.onclick = function(){
          html.classList.toggle('dark');
          iconLight.classList.toggle('hidden');
          iconDark.classList.toggle('hidden');
      }
      toggle2.onclick = function(){
          html.classList.toggle('dark');
          iconLight.classList.toggle('hidden');
          iconDark.classList.toggle('hidden');
      }
    })
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap');

/* html{
  background-color: #111111;
} */

#app {
  font-family: 'Roboto', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;
  width: 100vw;
}
</style>
