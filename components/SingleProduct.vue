<template>
  <div>
    <div class="relative single-product mx-2">
      <div class="relative">
        <img
          src="~/assets/images/product1.png"
          alt=""
          class="w-full h-full object-cover"
        />
        <div
          class="absolute product-info h-full w-full bottom-0 right-0 p-4 bg-opacity-50 bg-gray-600 rounded-xl overflow-hidden"
        >
          <div
            class="flex flex-col justify-center items-center w-full h-full text-2xl"
          >
            <div class="flex text-white gap-4 mb-6">
              <button class="w-12 h-12 rounded-full border border-2 shadow">
                +
              </button>
              <span
                class="w-12 h-12 rounded-full bg-white text-green-500 flex justify-center items-center"
              >
                0</span
              >
              <button class="w-12 h-12 rounded-full border border-2 shadow">
                -
              </button>
            </div>
            <button
              class="rounded-full text-white bg-green-500 text-base px-8 py-2 hover:text-white hover:bg-green-500 shadow"
            >
              Add to Cart
            </button>
            <div
              class="absolute bottom-0 w-full bg-gray-200 p-2 text-gray-600 text-lg text-center"
            >
              <button>Details <span class="hover:ml-4">&#8594;</span></button>
            </div>
          </div>
        </div>
      </div>
      <div
        class="absolute text-white top-0 right-0 m-2 bg-gray-800 px-3 text-sm py-1 rounded-full"
      >
        - 10%
      </div>
      <div class="text-center">
        <h3 class="py-2 text-xl">Product Name</h3>
        <p class="text-yellow-500">
          $200.00
          <span class="text-gray-400 line-through">$220.00</span>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SingleProduct',
}
</script>

<style></style>
