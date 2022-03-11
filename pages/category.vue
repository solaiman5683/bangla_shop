<template>
  <div class="container">
    <div class="flex py-8">
      <div class="w-1/4">
        <SideBar />
      </div>
      <div class="w-3/4 pl-4">
        <img class="w-full" src="~/assets/images/category-hero.png" alt="" />

        <section class="mt-6">
          <h3 class="text-3xl">Fruits Collection</h3>

          <div class="flex justify-between mt-4">
            <div class="flex text-gray-400">
              <button class="pr-4 border-r-2 text-lg">Fruits</button>
              <button class="px-4 border-r-2 text-lg">Green Fruits</button>
              <button class="pl-4 text-lg text-gray-800">Fresh Fruits</button>
            </div>
          </div>

          <div class="grid grid-cols-3 gap-6 py-8">
            <SingleProduct v-for="item in 3" />
          </div>
          <div class="text-center">
            <button
              class="bg-green-700 hover:bg-green-600 text-lg text-white px-6 py-2 rounded-full"
            >
              Load More
            </button>
          </div>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import SideBar from '~/components/SideBar.vue'
import SingleProduct from '../components/SingleProduct.vue'
export default {
  components: { SingleProduct },
}
</script>

<style></style>
