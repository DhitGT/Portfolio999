<template>
  <div :class="['max-w-fit', 'pe-4', 'items-center', dynamicWidth]">
    <div
      class="items-center gap-2 max-w-fit flex rounded-3xl bg-gray-100 pa-2 px-5"
      :class="[bgColor]"
    >
      <div v-if="!noImage">
        <v-img :style="{ width: imageSize }" :src="img"></v-img>
      </div>
      <span :class="['text-gray-900', fontSize, 'font-bold']">{{ name }}</span>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    img: {
      type: String, // Corrected 'Type' to 'type'
      default: 'https://placehold.co/300',
    },
    bgColor: {
      type: String,
      default: 'bg-gray-100',
    },
    noImage: {
      type: Boolean,
      default: false,
    },
    name: {
      type: String, // Corrected 'Type' to 'type'
    },
    width: {
      type: String, // Corrected 'Type' to 'type'
      default: '',
    },
  },
  computed: {
    dynamicWidth() {
      const widthClasses = {
        'x-small': 'h-1/5',
        small: 'h-1/2',
        large: 'h-3/4',
        'x-large': 'w-full',
      }
      return widthClasses[this.width] || '' // Return the corresponding class or an empty string
    },
    imageSize() {
      const widthClasses = {
        'x-small': '1em',
        small: '1.5em',
        large: '2.5em',
        'x-large': '3.em',
      }
      return widthClasses[this.width] || '1.5em'
    },
    fontSize() {
      const widthClasses = {
        'x-small': 'text-xs',
        small: 'text-sm',
        large: 'text-xl',
        'x-large': 'text-2xl',
      }
      return widthClasses[this.width] || ''
    },
  },
}
</script>
