<template>
  <button class="bg-gray-700 text-white py-2 px-4 rounded" :style="style">
    {{ text }}
  </button>
</template>
<script lang="ts">
  import Vue from 'vue'
  export default Vue.extend({
    props: {
      text: {
        required: true,
        type: String,
      },
      width: {
        default: 'auto',
        type: String,
      },
      height: {
        default: 'auto',
        type: String,
      },
    }
})
</script>