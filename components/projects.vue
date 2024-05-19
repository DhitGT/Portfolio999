<template>
  <div class="flex flex-col mt-24">
    <span class="text-4xl font-bold text-center text-orange-400"
      >Projects I've Worked On</span
    >
    <div class="flex flex-col gap-4 mt-12">
      <div
        v-for="(item, i) in item"
        :key="`proj-${i}`"
        class="pa-4 bg-gradient-to-t from-gray-800 to-blue-400 flex rounded-3xl"
      >
        <div class="left rounded-3xl w-1/2 aspect-video">
          <v-img
            class="rounded-2xl aspect-video"
            src="https://placehold.co/300"
          >
          </v-img>
        </div>
        <div class="flex flex-col gap-3">
          <div class="right flex flex-col gap-3 pa-3">
            <span class="text-3xl w-full font-bold">{{ item.title }}</span>
            <div class="py-2">
              <span class=""> Worked On </span>
              <div class="flex flex-wrap max-h-fit">
                <badge
                  :name="woItem"
                  width="x-small"
                  noImage="true"
                  bgColor="bg-gray-300"
                  v-for="(woItem, iwo) in item.workOn"
                  :key="`prod-wo-${iwo}-${i}`"
                />
              </div>
            </div>
            <div class="py-2">
              <span class=""> Technologies i have used </span>
              <div class="flex flex-wrap">
                <badge
                  :name="techitem.name"
                  width="x-small"
                  bgColor="bg-gray-300"
                  v-for="(techitem, techi) in item.tech"
                  :key="`prod-tech-${techi}-${i}`"
                />
              </div>
            </div>
            <v-btn outlined large rounded color="white" class="max-w-fit"
              >Go to {{ item.title }}</v-btn
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      item: [
        {
          title: 'Document Management System',
          workOn: ['website', 'admin panel'],
          url: '',
          tech: [
            { name: 'Nuxt 2', img: '' },
            { name: 'Vuetify 2', img: '' },
            { name: 'Tailwind Css', img: '' },
          ],
        },
      ],
    }
  },
}
</script>
