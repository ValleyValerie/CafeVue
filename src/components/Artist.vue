<script setup>
import { ref } from 'vue'

const badgeText = ref('Please Check out the Designer')
const badgeLink = ref('https://dribbble.com/shots/24513896-Coffee-Shop-Website') 
</script>

<template>
  <div class="relative p-2 bg-gray-100  flex items-center justify-center">
    <div class="flex items-center space-x-2">
     
      <a :href="badgeLink" class="inline-block rounded-full bg-indigo-900 px-3 py-1 text-white no-underline">
        {{ badgeText }}
      </a>
    </div>
  </div>
</template>


