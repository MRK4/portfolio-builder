<template>
  <div class="flex flex-col justify-center items-center text-center text-white space-y-9">
    <div class="space-y-6">

      <!-- PROFILE PICTURE -->
      <div class="flex flex-col justify-center items-center space-y-6">
        <img class="outline-2 border-4 border-cta shadow-lg shadow-cta/50 w-auto h-48 rounded-full" src="@/assets/imgs/avatar.jpg" alt="Profile Picture">
        <div class="space-y-2">
          <!-- CUSTOMISATION: Change your name here -->
          <h1 class="text-4xl font-semibold text-customblack dark:text-white">John Smith</h1>
          <!-- CUSTOMISATION: Change your job here -->
          <h2 class="text-lg text-customgray">Photographer</h2>
        </div>
      </div>

      <div class="space-y-3">
        <!-- SOCIAL MEDIAS -->
        <div class="flex flex-row justify-between items-center space-x-6">
          <a class="transition-all ease-in-out duration-150 transform p-1 text-cta hover:text-customblack dark:hover:text-white hover:scale-125" href="">
            <i class="fa-brands fa-instagram fa-xl"></i>
          </a>
          <a class="transition-all ease-in-out duration-150 transform p-1 text-cta hover:text-customblack dark:hover:text-white hover:scale-125" href="">
            <i class="fa-brands fa-linkedin fa-xl"></i>
          </a>
          <a class="transition-all ease-in-out duration-150 transform p-1 text-cta hover:text-customblack dark:hover:text-white hover:scale-125" href="">
            <i class="fa-brands fa-twitter fa-xl"></i>
          </a>
          <a class="transition-all ease-in-out duration-150 transform p-1 text-cta hover:text-customblack dark:hover:text-white hover:scale-125" href="">
            <i class="fa-brands fa-tiktok fa-xl"></i>
          </a>
          <a class="transition-all ease-in-out duration-150 transform p-1 text-cta hover:text-customblack dark:hover:text-white hover:scale-125" href="">
            <i class="fa-brands fa-facebook fa-xl"></i>
          </a>
        </div>

        <!-- ADDITIONAL INFO -->
        <div>
          <!-- CUSTOMISATION: Add some details -->
          <p class="text-sm text-customgray">additional info here...</p>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'Portfolio_Header'
}
</script>

<style scoped>
</style>
