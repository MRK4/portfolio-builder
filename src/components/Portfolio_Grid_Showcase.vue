<template>
  <div class="grid grid-cols-3 gap-4 h-full w-full">

    <a v-for="project in projects" :key="project" :href="project.url">
      <div class="group transition-all select-none ease-in-out duration-150 w-auto h-auto items-center justify-center relative">
        <img class="group-hover:blur-sm inset-0 z-0" :src="require(`@/assets/thumbnails/${project.img}`)" alt="">
        <div class="group-hover:blur-none blur-none opacity-0 hover:opacity-100 duration-300 absolute inset-0 z-10 flex justify-center items-center text-6xl text-white font-semibold drop-shadow text-center">{{ project.title }}</div>
      </div>
    </a>

  </div>
</template>

<script>
export default {
  name: 'Portfolio_Grid_Showcase',
  data() {
    return {
      projects: [
        {
          title: "Project Title 1",
          img: "img1.jpg",
          url: "https://www.google.com",
        },
        {
          title: "Project Title 2",
          img: "img2.jpg",
          url: "https://www.google.com",
        },
        {
          title: "Project Title 2",
          img: "img3.jpg",
          url: "https://www.google.com",
        },
        {
          title: "Project Title 2",
          img: "img4.jpg",
          url: "https://www.google.com",
        },
        {
          title: "Project Title 2",
          img: "img5.jpg",
          url: "https://www.google.com",
        },
      ]
    }
  }
}
</script>

<style>
</style>
