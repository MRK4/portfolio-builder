<template>
  <footer>
    <p class="text-center text-customdarkmodebg dark:text-white opacity-50">{{ nickname }} &copy; {{ year }}</p>
    <!-- You're NOT allowed to change this line, be careful >:( -->
    <p class="text-center text-sm text-customdarkmodebg dark:text-white opacity-25">Template by MRK</p>
  </footer>
</template>

<script>
export default {
  name: 'Portfolio_Footer',
  data() {
    return {
      // CUSTOMISATION: Change your name here
      nickname: "Jhon Smith",
      // CUSTOMISATION: Change your year here
      year: "2022"
    }
  }
}
</script>

<style>
</style>
