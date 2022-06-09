<template>
  <main>
    <div class="flex fixed top-2 justify-center w-full">
      <div
        class="z-50 w-48 text-2xl text-center text-white bg-red-700 border-2 border-white"
      >
        <div class="block sm:hidden">
          XS
        </div>
        <div class="hidden sm:block md:hidden">
          SM
        </div>
        <div class="hidden md:block lg:hidden">
          MD
        </div>
        <div class="hidden lg:block xl:hidden">
          LG
        </div>
        <div class="hidden xl:block 2xl:hidden">
          XL
        </div>
        <div class="hidden 2xl:block">
          2XL
        </div>
      </div>
    </div>
    <slot name="bloks" />
  </main>
</template>

<script>
export default {
  props: {
    blok: {
      type: Object,
      default: () => ({})
    }
  }
}
</script>
