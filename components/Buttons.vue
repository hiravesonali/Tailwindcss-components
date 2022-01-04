<template>
  <div
    class="min-h-screen bg-gray-900 py-6 flex flex-col justify-center relative overflow-hidden sm:py-12"
  >
    <div
      class="flex flex-col my-10 bg-gray-700 backdrop-blur ring-1 ring-inset ring-gray-500/20 h-28 w-64 mx-auto rounded-lg cursor-context-menu"
    >
      <!-- Button Snippet -->
      <div class="m-auto text-gray-200">
        <div
          class="px-6 py-3 bg-indigo-500 text-white font-semibold rounded-lg border-b-4 border-b-indigo-200 hover:border-b-0 transition-all ease-in-out duration-100"
        >
          Hover over me
        </div>
      </div>
      <div class="m-auto text-gray-200">
        <div
          class="px-6 py-3 bg-indigo-500 text-white font-semibold rounded-lg border-b-4 border-b-indigo-200 hover:border-b-0 transition-all ease-in-out duration-100"
        >
          Hover over me
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'ButtonsComponent',
  data() {
    return {
      showMobileMenu: false,
    }
  },
}
</script>
