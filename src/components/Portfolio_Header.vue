<template>
  <div class="flex flex-col justify-center items-center text-center text-white space-y-9">
    <div class="space-y-6">

      <!-- PROFILE PICTURE -->
      <div class="flex flex-col justify-center items-center space-y-6">
        <img class="outline-2 border-4 border-cta shadow-lg shadow-cta/50 w-auto h-48 rounded-full" src="@/assets/imgs/avatar.jpg" alt="Profile Picture">
        <div class="space-y-2">
          <h1 class="text-4xl font-semibold text-customblack dark:text-white">{{ nickname }}</h1>
          <h2 class="text-lg text-customgray">{{ job }}</h2>
        </div>
      </div>

      <div class="space-y-3">
        <!-- SOCIAL MEDIAS -->
        <div class="flex flex-row justify-between items-center space-x-6">
          <a v-for="social in socials" :key="social" :href="social.url" class="transition-all ease-in-out duration-150 transform p-1 text-cta hover:text-customblack dark:hover:text-white hover:scale-125">
            <i class="fa-brands fa-xl" :class="`fa-${social.name}`"></i>
          </a>
        </div>

        <!-- ADDITIONAL INFO -->
        <div>
          <p class="text-sm text-customgray"> {{ details }} </p>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'Portfolio_Header',
  data() {
    return {
      socials: [
        // CUSTOMISATION: Add your social networks, there's an example at the end
        // Copy & Paste and then add your infos !
        {
          name: "instagram",
          url: "https://www.google.com",
        },
        {
          name: "tiktok",
          url: "https://www.google.com",
        },
        {
          name: "facebook",
          url: "https://www.google.com",
        },
        {
          name: "linkedin",
          url: "https://www.google.com",
        },
        {
          name: "youtube",
          url: "https://www.google.com",
        },
      ],
      // CUSTOMISATION: Change your name here
      nickname: "Jhon Smith",
      // CUSTOMISATION: Change your job here
      job: "Photographer",
      // CUSTOMISATION: Add some details
      details: "additional info here..."
    }
  }
}
</script>

<style scoped>
</style>
