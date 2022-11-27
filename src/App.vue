<script setup>
import { ref, onMounted } from 'vue'

const backgroundColor = ref('#ff0000')

const setBackgroundColor = () => {
  document.querySelector('body').style.backgroundColor = backgroundColor.value;
}
</script>

<template>
<div>
  <div>
    <input type="text" v-model="backgroundColor" />
    <button @click="setBackgroundColor">
      Change background
    </button>
  </div>
</div>
</template>