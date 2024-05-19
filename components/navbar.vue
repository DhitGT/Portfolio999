<template>
  <div
    class="bg-gray-200 fixed top-5 left-1/2 transform -translate-x-1/2 z-50 w-[80vw] pa-3 items-center rounded-full flex"
  >
    <div class="flex items-center gap-2">
      <div class="">
        <v-img
          style="width: 1.7em"
          class="rounded-full"
          src="https://placehold.co/300/000000/FFF"
        >
        </v-img>
      </div>
      <span class="text-gray-900"
        >Aditya <span class="font-bold">Dwi</span></span
      >
    </div>
    <div
      style="max-width: fit-content"
      class="flex pa-0 bg-gray-900 items-center justify-center rounded-3xl ps-3 ml-auto"
    >
      <span class="ma-0 text-xs mr-3 text-white">Menu</span>
      <v-btn icon fab class="pa-0 ma-0 bg-orange-600" x-small>
        <v-icon>mdi-menu</v-icon>
      </v-btn>
    </div>
  </div>
</template>
