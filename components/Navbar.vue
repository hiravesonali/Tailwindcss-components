<template>
  <div>
    <div class="max-w-screen-xl mx-auto px-4 pb-1 sm:px-6">
      <nav
        class="relative flex items-center justify-between sm:h-10 md:justify-center"
      >
        <div
          class="flex items-center flex-1 md:absolute md:inset-y-0 md:left-0"
        >
          <div class="flex items-center justify-between w-full md:w-auto">
            <a
              class="text-lg px-1 border border-white rounded font-bold text-white"
              href="/"
            >
              Tailwind Blocks
            </a>
            <div class="-mr-2 flex items-center md:hidden">
              <button
                @click="showMobileMenu = true"
                type="button"
                class="inline-flex items-center justify-center p-2 rounded-md text-white hover:text-gray-100 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-100 transition duration-150 ease-in-out"
              >
                <svg
                  class="h-6 w-6"
                  stroke="currentColor"
                  fill="none"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M4 6h16M4 12h16M4 18h16"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>

        <div
          class="hidden md:absolute md:flex md:items-center md:justify-end md:inset-y-0 md:right-0"
        >
          <span class="inline-flex">
            <div class="flex justify-center mt-3 md:order-2">
              <a
                href="https://github.com/hiravesonali"
                class="ml-6 text-gray-100 hover:text-gray-200"
                target="_blank"
              >
                <span class="sr-only">Github</span>
                <svg class="h-8 w-8" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    fill-rule="evenodd"
                    d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"
                    clip-rule="evenodd"
                  />
                </svg>
              </a>
              <a
                href="https://twitter.com/ShonaDesign"
                class="ml-6 text-gray-100 hover:text-gray-200"
                target="https://twitter.com/ShonaDesign"
              >
                <span class="sr-only">Twitter</span>
                <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M8.29 20.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0022 5.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.072 4.072 0 012.8 9.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 012 18.407a11.616 11.616 0 006.29 1.84"
                  />
                </svg>
              </a>
            </div>
          </span>
        </div>
      </nav>
    </div>
    <!-- Mobile menu starts here -->
    <div
      v-show="showMobileMenu"
      class="absolute top-0 inset-x-0 p-2 z-50 md:hidden"
    >
      <div
        class="rounded-lg shadow-md transition transform origin-top-right"
        x-transition:enter="duration-150 ease-out"
        x-transition:enter-start="opacity-0 scale-95"
        x-transition:enter-end="opacity-100 scale-100"
        x-transition:leave="duration-100 ease-in"
        x-transition:leave-start="opacity-100 scale-100"
        x-transition:leave-end="opacity-0 scale-95"
      >
        <div class="rounded-lg bg-white shadow-xs overflow-hidden">
          <div class="px-5 pt-4 flex items-center justify-between">
            <div>
              <logo />
            </div>
            <div class="-mr-2">
              <button
                @click="showMobileMenu = false"
                type="button"
                class="inline-flex items-center justify-center p-2 rounded-md text-white hover:text-gray-100 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-100 transition duration-150 ease-in-out"
              >
                <svg
                  class="h-6 w-6"
                  stroke="currentColor"
                  fill="none"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M6 18L18 6M6 6l12 12"
                  />
                </svg>
              </button>
            </div>
          </div>
          <div>
            <div class="flex justify-center pb-5">
              <a
                href="https://github.com/hiravesonali"
                class="ml-6 text-gray-100 hover:text-gray-200"
                target="_blank"
              >
                <span class="sr-only">Github</span>
                <svg class="h-8 w-8" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    fill-rule="evenodd"
                    d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"
                    clip-rule="evenodd"
                  />
                </svg>
              </a>
              <a
                href="https://twitter.com/ShonaDesign"
                class="ml-6 text-gray-100 hover:text-gray-200"
                target="https://twitter.com/ShonaDesign"
              >
                <span class="sr-only">Twitter</span>
                <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M8.29 20.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0022 5.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.072 4.072 0 012.8 9.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 012 18.407a11.616 11.616 0 006.29 1.84"
                  />
                </svg>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavbarComponent',
  data() {
    return {
      showMobileMenu: false,
    }
  },
}
</script>
