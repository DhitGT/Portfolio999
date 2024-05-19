<template>
  <div class="my-12">
    <div class="flex justify-center">
      <span class="text-4xl font-bold text-orange-400">Skills</span>
    </div>
    <div class="flex flex-col items-center gap-12 justify-center my-12">
      <span class="text-3xl font-bold text-orange-400">Design Tools I Use</span>
      <badge name="Figma" />
    </div>
    <div class="flex flex-col items-center gap-12 justify-center my-12">
      <span class="text-3xl font-bold text-orange-400">Thecnologies I Use</span>
      <div class="flex flex-wrap justify-center items-center gap-3">
        <badge :name="item.name" v-for="(item, i) in tech" :key="`tech-${i}`" />
      </div>
    </div>
    <div class="flex flex-col items-center gap-12 justify-center my-12">
      <span class="text-3xl font-bold text-orange-400"
        >DEVELOPMENT & PRODUCTIVITY TOOLS I USE</span
      >
      <div class="flex flex-wrap justify-center items-center gap-3">
        <badge
          :name="item.name"
          v-for="(item, i) in tools"
          :key="`tools-${i}`"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      tech: [
        {
          img: '',
          name: 'HTML',
        },
        {
          img: '',
          name: 'CSS',
        },
        {
          img: '',
          name: 'Javascript',
        },
        {
          img: '',
          name: 'HTML',
        },
        {
          img: '',
          name: 'CSS',
        },
        {
          img: '',
          name: 'Javascript',
        },
        {
          img: '',
          name: 'HTML',
        },
        {
          img: '',
          name: 'CSS',
        },
        {
          img: '',
          name: 'Javascript',
        },
        {
          img: '',
          name: 'HTML',
        },
        {
          img: '',
          name: 'CSS',
        },
        {
          img: '',
          name: 'Javascript',
        },
        {
          img: '',
          name: 'HTML',
        },
        {
          img: '',
          name: 'CSS',
        },
        {
          img: '',
          name: 'Javascript',
        },
        {
          img: '',
          name: 'HTML',
        },
        {
          img: '',
          name: 'CSS',
        },
        {
          img: '',
          name: 'Javascript',
        },
      ],
      tools: [
        {
          img: '',
          name: 'Visual Studio Code',
        },
        {
          img: '',
          name: 'Github',
        },
        {
          img: '',
          name: 'Notion',
        },
        {
          img: '',
          name: 'Postman',
        },
      ],
    }
  },
}
</script>
