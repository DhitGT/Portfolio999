<template>
  <div class="flex flex-col mt-24">
    <span class="text-3xl font-bold text-center text-orange-400"
      >Experience</span
    >
    <div class="flex flex-col gap-4 mt-12">
      <div
        v-for="(item, i) in item"
        :key="`exp-${i}`"
        class="pa-4 bg-gray-100 rounded-3xl"
      >
        <div class="flex justify-between">
          <div
            class="flex gap-3 pe-6 bg-gray-900 rounded-full items-center"
            style="max-width: fit-content"
          >
            <div>
              <v-img
                style="width: 2.5em"
                class="rounded-full"
                src="https://placehold.co/300"
              ></v-img>
            </div>
            <div class="flex py-1 flex-col justify-center">
              <span class="text-orange-400 font-bold text-sm">
                {{ item.office }}
              </span>
              <div class="flex gap-2">
                <v-icon small>mdi-map-marker</v-icon>
                <span class="text-xs">{{ item.location }}</span>
              </div>
            </div>
          </div>
          <div
            class="flex gap-3 px-6 bg-orange-200 rounded-full items-center"
            style="max-width: fit-content; max-height: fit-content"
          >
            <div class="flex flex-col justify-center">
              <div class="flex gap-2">
                <v-icon small color="black">mdi-calendar</v-icon>
                <span class="text-xs text-gray-900 font-extrabold">{{
                  item.date
                }}</span>
              </div>
            </div>
          </div>
        </div>
        <div class="flex items-center gap-3 mt-5">
          <div>
            <v-img
              src="https://placehold.co/300"
              style="width: 2.5em"
              class="rounded-full"
            ></v-img>
          </div>
          <span class="font-bold text-xl text-gray-900">{{
            item.division
          }}</span>
        </div>
        <div
          class="flex flex-col pa-3 gap-3"
          v-for="(itemtask, itask) in item.task"
          :key="`task-${itask}`"
        >
          <div class="flex gap-3">
            <v-icon small color="black">mdi-send-outline</v-icon>
            <span class="text-gray-900">{{ itemtask }}</span>
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
          office: 'PT traspac makmur sejahtera',
          location: 'Central Jakarta',
          date: 'FEB 2024 - AUGUST 2024',
          division: 'Intern Fullstack Developer',
          task: [
            'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nobis laborum aliquid neque ea rerum rem?',
            'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ad    neque quidem officiis iusto consequuntur eveniet omnis            perspiciatis aliquam minima perferendis',
          ],
        },
        {
          office: 'PT traspac makmur sejahtera',
          location: 'Central Jakarta',
          date: 'FEB 2024 - AUGUST 2024',
          division: 'Intern Fullstack Developer',
          task: [
            'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nobis laborum aliquid neque ea rerum rem?',
            'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ad    neque quidem officiis iusto consequuntur eveniet omnis            perspiciatis aliquam minima perferendis',
          ],
        },
      ],
    }
  },
}
</script>
