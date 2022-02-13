<template>
  <div class="container py-6">
    <div class="mb-6 flex justify-between items-center">
      <!--  Logo -->
      <nuxt-link to="/" class="flex items-center gap-4">
        <img src="~/assets/images/logo.svg" width="65px" alt="Bangla Store" />
        <h3 class="text-3xl">Bangla Shop</h3>
      </nuxt-link>
      <div class="w-96">
        <div
          class="border border-gray-200 p-1 flex rounded-full min-w-max items-center"
        >
          <div class="min-w-max p-2">
            <img src="~/assets/images/search.svg" alt="search_icon" />
          </div>
          <input
            class="p-2 focus:outline-none"
            type="search"
            placeholder="Search Here.... "
          />
          <button class="bg-gray-700 py-3 px-7 rounded-full text-white">
            Search
          </button>
        </div>
      </div>

      <div class="min-w-max flex">
        <nuxt-link to="/" class="w-14 h-14 hover:bg-gray-100 p-4 rounded-full">
          <img src="~/assets/images/heart.svg" alt="" />
        </nuxt-link>
        <nuxt-link class="relative" to="/">
          <span
            class="w-14 h-14 hover:bg-gray-100 p-4 rounded-full flex items-center justify-center"
          >
            <img src="~/assets/images/cart.svg" alt="" />
          </span>
          <span
            class="absolute w-4 h-4 top-0 right-0 bg-red-500 text-sm text-white p-3 flex justify-center items-center rounded-full"
            >0</span
          >
        </nuxt-link>
        <nuxt-link to="/" class="flex items-center gap-1">
          <span
            class="w-14 h-14 hover:bg-gray-100 p-4 rounded-full flex items-center justify-center"
          >
            <img src="~/assets/images/avater.svg" alt="" />
          </span>
          Account
        </nuxt-link>
      </div>
    </div>
    <div class="flex items-center">
      <div v-click-outside="closeCategory" class="relative">
        <div
          @click.prevent="toggleCategory"
          class="w-96 z-20 relative bg-green-500 cursor-pointer text-white py-4 px-6 rounded-full flex justify-between items-center"
        >
          <div class="min-w-max">
            <img src="~/assets/images/menu-right.svg" alt="" />
          </div>
          <span>All Category</span>
          <div class="min-w-max">
            <img src="~/assets/images/chevron-down.svg" alt="" />
          </div>
        </div>

        <!-- Category Menu -->
        <div
          v-bind:class="
            isCategoryOpen ? 'block visible w-full ' : 'hidden invisible w-0'
          "
          class="absolute top-10 rounded-b-2xl transition ease-in-out -mt-4 z-10 bg-green-500"
        >
          <ul class="pt-6 pb-4">
            <li>
              <nuxt-link class="block px-6 py-2 text-white" to="/"
                >Fruits</nuxt-link
              >
            </li>
            <li>
              <nuxt-link class="block px-6 py-2 text-white" to="/"
                >Fruits</nuxt-link
              >
            </li>
            <li>
              <nuxt-link class="block px-6 py-2 text-white" to="/"
                >Fruits</nuxt-link
              >
            </li>
            <li>
              <nuxt-link class="block px-6 py-2 text-white" to="/"
                >Fruits</nuxt-link
              >
            </li>
            <li>
              <nuxt-link class="block px-6 py-2 text-white" to="/"
                >Fruits</nuxt-link
              >
            </li>
            <li>
              <nuxt-link class="block px-6 py-2 text-white" to="/"
                >Fruits</nuxt-link
              >
            </li>
          </ul>
        </div>
      </div>
      <div class="w-full">
        <ul class="flex justify-center gap-16">
          <li>
            <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/">Shop</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/">Pages</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/">Blogs</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/">Contact</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/">Trace Order</nuxt-link>
          </li>
        </ul>
      </div>
      <div class="min-w-max">
        <p class="flex items-center cursor-pointer" style="color: #ff5c00">
          <img src="~/assets/images/percentage.svg" alt="" /><span
            >Special Offers!</span
          >
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      isCategoryOpen: false,
    }
  },
  methods: {
    toggleCategory() {
      this.isCategoryOpen = !this.isCategoryOpen
    },
    closeCategory() {
      this.isCategoryOpen = false
    },
  },
}
</script>

<style></style>
