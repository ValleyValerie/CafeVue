<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

import {
  Dialog, 
  DialogPanel, 
  Disclosure, 
  DisclosureButton, 
  DisclosurePanel, 
  Popover, 
  PopoverButton, 
  PopoverGroup, 
  PopoverPanel
} from '@headlessui/vue'

import {
  ArrowPathIcon, 
  Bars3Icon, 
  ChartPieIcon, 
  CursorArrowRaysIcon, 
  FingerPrintIcon, 
  SquaresPlusIcon, 
  XMarkIcon
} from '@heroicons/vue/24/outline'

import { 
  ChevronDownIcon, 
  PhoneIcon, 
  PlayCircleIcon 
} from '@heroicons/vue/20/solid'

const isScrolled = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 0
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})

const mobileMenuOpen = ref(false)
</script>

<template>
  <header :class="['fixed w-full z-50 transition-shadow', isScrolled ? 'shadow-lg bg-white' : 'bg-transparent']">
    <nav class="mx-auto flex max-w-7xl items-center p-8 lg:px-8" aria-label="Global">
      <div class="flex lg:hidden">
        <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700" @click="mobileMenuOpen = true">
          <span class="sr-only">Open main menu</span>
          <Bars3Icon class="h-6 w-6" aria-hidden="true" />
        </button>
      </div>
      <PopoverGroup class="hidden lg:flex lg:flex-grow lg:justify-between">
        <a href="#home" class="font-semibold leading-6 text-3xl italic font-crimson hover:bg-gray-200 hover:text-amber-600">Home</a>
        <a href="#menu" class="font-semibold leading-6 text-3xl italic font-crimson hover:bg-gray-200 hover:text-amber-600">Menu</a>
        <a href="#about" class="text-3xl font-semibold leading-6 italic font-crimson hover:bg-gray-200 hover:text-amber-600">About</a>
        <a href="#location" class="text-3xl font-semibold leading-6 italic font-crimson hover:bg-gray-200 hover:text-amber-600">Location</a>
      </PopoverGroup>
    </nav>
    <Dialog class="lg:hidden" @close="mobileMenuOpen = false" :open="mobileMenuOpen">
      <div class="fixed inset-0 z-10" />
      <DialogPanel class="fixed inset-y-0 right-0 z-10 w-full overflow-y-auto bg-white px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10">
        <div class="flex items-center justify-between">
          <button type="button" class="-m-2.5 rounded-md p-2.5 text-gray-700" @click="mobileMenuOpen = false">
            <span class="sr-only">Close menu</span>
            <XMarkIcon class="h-6 w-6" aria-hidden="true" />
          </button>
        </div>
        <div class="mt-6 flow-root">
          <div class="-my-6 divide-y divide-gray-500/10">
            <div class="space-y-2 py-6">
              <a href="#home" class="text-2xl -mx-3 block rounded-lg px-3 py-2 font-semibold leading-7 italic font-crimson hover:bg-gray-200 hover:text-amber-600">Home</a>
              <a href="#menu" class="text-2xl -mx-3 block rounded-lg px-3 py-2 font-semibold leading-7 italic font-crimson hover:bg-gray-200 hover:text-amber-600">Menu</a>
              <a href="#about" class="text-2xl -mx-3 block rounded-lg px-3 py-2 font-semibold leading-7 italic font-crimson hover:bg-gray-200 hover:text-amber-600">About</a>
              <a href="#location" class="text-2xl -mx-3 block rounded-lg px-3 py-2 font-semibold leading-7 italic font-crimson hover:bg-gray-200 hover:text-amber-600">Location</a>
            </div>
          </div>
        </div>
      </DialogPanel>
    </Dialog>
  </header>
</template>

<style>
html {
  scroll-behavior: smooth;
}
section {
  min-height: 100vh; 
  padding-top: 60px; 
}
</style>
