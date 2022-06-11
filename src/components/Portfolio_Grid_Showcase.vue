<template>
  <div class="grid grid-cols-1 sm:grid-cols-2 lg:sm:grid-cols-3 gap-4 h-full w-full">

    <a v-for="project in projects" :key="project" :href="project.url" class="space-y-3">
      <div class="group transition-all select-none ease-in-out duration-150 w-auto h-auto items-center justify-center relative">
        <img class="group-hover:blur-sm inset-0 z-0" :src="require(`@/assets/thumbnails/${project.img}`)" alt="">
        <div class="group-hover:blur-none blur-none opacity-0 hover:opacity-100 duration-300 absolute inset-0 z-10 flex justify-center items-center text-6xl text-white font-semibold drop-shadow text-center">{{ project.title }}</div>
      </div>
      <div class="text-center text-customblack dark:text-white text-2xl font-semibold drop-shadow sm:hidden">{{ project.title }}</div>
    </a>

  </div>
</template>

<script>
export default {
  name: 'Portfolio_Grid_Showcase',
  data() {
    return {
      projects: [
        // CUSTOMISATION: Add your work here, there's an example at the end
        // Copy & Paste and then add your infos !
        // Please, don't forget that your images must be square (1000 x 1000, 2500 x 2500, 5000 x 5000, ...)
        {
          title: "Project Title",
          img: "img1.jpg",
          url: "https://www.pexels.com/fr-fr/photo/plafond-a-l-interieur-vieil-immeuble-classique-12318288/",
        },
        {
          title: "Project Title",
          img: "img2.jpg",
          url: "https://www.pexels.com/fr-fr/photo/lumineux-ville-route-gens-12190737/",
        },
        {
          title: "Project Title",
          img: "img3.jpg",
          url: "https://www.pexels.com/fr-fr/photo/parcs-de-vehicules-noirs-a-cote-d-un-batiment-en-beton-gris-1853540/",
        },
        {
          title: "Project Title",
          img: "img4.jpg",
          url: "https://www.pexels.com/fr-fr/photo/passons-la-nuit-ensemble-texte-sur-la-fenetre-en-verre-3607650/",
        },
        {
          title: "Project Title",
          img: "img5.jpg",
          url: "https://www.pexels.com/fr-fr/photo/photo-d-ampoule-pendentif-750843/",
        },
      ]
    }
  }
}
</script>

<style>
</style>
