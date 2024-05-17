<template>
  <div
    class="flex flex-col items-center mt-20 justify-center"
    style="z-index: 99"
  >
    <div class="flex items-center gap-2">
      <v-img src="">😋</v-img>
      <span class="text-3xl font-bold">
        Hello! I'm <span class="text-orange-300">Aditya Dwi Saputra</span>
      </span>
    </div>
    <span class="font-bold mt-3">A Frontend Developer | Web Developer</span>
    <div class="flex">
      <span>With</span>
      <span
        class="bg-gray-800 rounded-2xl font-bold text-orange-300 outline-1 mx-1 px-2"
        >2+ Years</span
      >
      <span>Learning Experience</span>
    </div>
    <div class="flex gap-4 mt-4 pt-2" style="z-index: 99">
      <v-btn color="#feb901" class="backdrop-blur-xl" rounded outlined>
        <v-icon color="#feb901">mdi-download-outline</v-icon>
        <span class="ms-1 text-[#feb901]">Resume</span>
      </v-btn>
      <v-btn color="#feb901" class="backdrop-blur" rounded>
        <span class="ms-1 text-[#191201]">Contact</span>
      </v-btn>
    </div>
  </div>
</template>
