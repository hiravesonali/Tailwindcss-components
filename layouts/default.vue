<template>
  <div
    class="text-body font-body overflow-auto bg-gradient-to-tl from-indigo-700 via-purple-800 to-indigo-900"
  >
    <div class="relative overflow-hidden">
      <div class="relative pt-6 pb-12 sm:pb-16 md:pb-20 lg:pb-28 xl:pb-32">
        <Navbar />
        <nuxt />
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'DefaultPage',
}
</script>
