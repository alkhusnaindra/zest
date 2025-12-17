<script setup>
import notFoundImage from "../assets/images/404-image.png";
</script>

<template>
  <div class="min-h-screen flex items-center justify-center">
    <!-- Wrapper -->
    <div
      class="flex flex-col md:flex-row items-center gap-8 md:gap-10
             max-w-5xl w-full px-6"
    >

      <div class="w-full md:w-1/2 flex justify-center md:mb-6 -mt-40 md:-mt-0">
        <img
          :src="notFoundImage"
          alt="404"
          class="w-100 md:w-125"
        />
      </div>

      <div
        class="w-full md:w-1/2 flex flex-col
               items-center md:items-start
               text-center md:text-left -mt-28 md:mt-0"
      >
        <p class="mt-4 text-3xl font-bold text-primary">
          Oops!, Page not found
        </p>

        <p class="mt-1 text-xl text-neutral-700 max-w-md">
          This page is missing or you assembled the link incorrectly
        </p>

        <router-link
          to="/"
          class="mt-10 md:mt-4 mx-auto md:mx-0 w-fit"
        >
          <div
            class="px-4 py-2 border-3 border-primary rounded-full
                   hover:bg-primary hover:text-white transition
                   text-primary"
          >
            Go Back Home
          </div>
        </router-link>
      </div>

    </div>
  </div>
</template>
