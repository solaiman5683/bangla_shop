<template>
  <div class="">
    <div class="container flex gap-4 my-14">
      <div class="w-1/4 flex gap-3 items-center">
        <div class="min-w-max">
          <img
            width="100px"
            height="100px"
            src="~/assets/images/support.svg"
            alt=""
          />
        </div>
        <div>
          <h3 class="text-2xl font-medium mb-4">24 Customer Support</h3>
          <p class="text-gray-400">Contact us 24 hours</p>
        </div>
      </div>
      <div class="w-1/4 flex gap-3 items-center">
        <div class="min-w-max">
          <img
            width="100px"
            height="100px"
            src="~/assets/images/products.svg"
            alt=""
          />
        </div>
        <div>
          <h3 class="text-2xl font-medium mb-4">Authentic Products</h3>
          <p class="text-gray-400">Contact us 24 hours</p>
        </div>
      </div>
      <div class="w-1/4 flex gap-3 items-center">
        <div class="min-w-max">
          <img
            width="100px"
            height="100px"
            src="~/assets/images/secure-pay.svg"
            alt=""
          />
        </div>
        <div>
          <h3 class="text-2xl font-medium mb-4">Secure Payment</h3>
          <p class="text-gray-400">Contact us 24 hours</p>
        </div>
      </div>
      <div class="w-1/4 flex gap-3 items-center">
        <div class="min-w-max">
          <img
            width="100px"
            height="100px"
            src="~/assets/images/offers.svg"
            alt=""
          />
        </div>
        <div>
          <h3 class="text-2xl font-medium mb-4">Best Prices & Offers</h3>
          <p class="text-gray-400">Contact us 24 hours</p>
        </div>
      </div>
    </div>

    <div class="bg-gray-100">
      <div class="container flex py-20">
        <div class="w-2/4">
          <nuxt-link to="/" class="flex items-center gap-4 mb-6">
            <img
              src="~/assets/images/logo.svg"
              width="65px"
              alt="Bangla Store"
            />
            <h3 class="text-3xl">Bangla Shop</h3>
          </nuxt-link>
          <p class="text-gray-400 w-3/4">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla diam
            ornare nam est gravida. Netus viverra rhoncus sit magna sapien ac
            eget parturient id. Est luctus dapibus quam aliquam in nisl turpis.
            Elit et dictum lacus morbi nec accumsan a in.
          </p>
          <div class="mt-6 flex cursor-pointer">
            <img src="~/assets/images/appstore.png" alt="" />
            <img src="~/assets/images/playstore.png" alt="" />
          </div>
        </div>

        <div class="w-1/4">
          <h3 class="text-2xl font-medium text-gray-600 mb-6">About Us</h3>
          <ul class="about-links">
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                About Karte
              </nuxt-link>
            </li>
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Contact
              </nuxt-link>
            </li>
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Career
              </nuxt-link>
            </li>
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Terms & Conditions
              </nuxt-link>
            </li>
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Category
              </nuxt-link>
            </li>
          </ul>
        </div>

        <div class="w-1/4">
          <h3 class="text-2xl font-medium text-gray-600 mb-6">Info</h3>
          <ul class="about-links">
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Information
              </nuxt-link>
            </li>
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Shipping
              </nuxt-link>
            </li>
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Payments
              </nuxt-link>
            </li>
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Return
              </nuxt-link>
            </li>
            <li class="mb-4">
              <nuxt-link to="/about" class="text-gray-400 hover:text-gray-500">
                Blog
              </nuxt-link>
            </li>
          </ul>
        </div>
      </div>

      <div class="container flex pb-4 justify-between items-center">
        <div class="min-w-max">
          <ul class="flex">
            <li
              class="hover:bg-red-400 bg-white mr-2 rounded shadow hover:text-white"
            >
              <a class="p-3 block" href="#">
                <i class="fa-brands fa-facebook-f"></i>
              </a>
            </li>
            <li
              class="hover:bg-red-400 bg-white mr-2 rounded shadow hover:text-white"
            >
              <a class="p-3 block" href="#"
                ><i class="fa-brands fa-instagram"></i
              ></a>
            </li>
            <li
              class="hover:bg-red-400 bg-white mr-2 rounded shadow hover:text-white"
            >
              <a class="p-3 block" href="#"
                ><i class="fa-brands fa-twitter"></i
              ></a>
            </li>
            <li
              class="hover:bg-red-400 bg-white mr-2 rounded shadow hover:text-white"
            >
              <a class="p-3 block" href="#"
                ><i class="fa-brands fa-skype"></i
              ></a>
            </li>
          </ul>
        </div>
        <div class="min-w-max">
          <p class="text-gray-400">
            @2022 Copyright All Right Reserved by Bengal Shop
          </p>
        </div>
        <div class="min-w-max">
          <img src="~/assets/images/pay-options.png" alt="" />
        </div>
      </div>
    </div>

    <!-- Product details modal -->
    <div
      v-if="modal"
      class="fixed w-full h-full min-h-screen z-30 top-0 left-0"
    >
      <div
        @click.prevent="modalClose"
        class="absolute bg-gray-800 opacity-60 h-full w-full top-0 left-0"
      ></div>
      <div
        class="w-4/6 bg-white shadow-2xl rounded-2xl p-8 relative mx-auto z-30 my-10 relative"
      >
        <svg
          @click.prevent="modalClose"
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6 absolute right-5 top-5 cursor-pointer"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M6 18L18 6M6 6l12 12"
          />
        </svg>

        <div class="flex -mx-8">
          <div class="w-1/2 px-8">
            <img src="product.image" />
          </div>
          <div class="w-1/2 px-8">
            <p class="text-sm mb-3">
              <span class="uppercase text-gray-400 pr-6">Status</span>
              <span class="bs-dark-green-color">In Stock</span>
            </p>
            <h3 class="text-2xl">
              <!-- {{ product.name }} -->
              Hello
            </h3>
            <p class="text-xs text-gray-400 mb-4 mt-2">
              <b>7</b> items available.
            </p>
            <p class="text-2xl font-bold">
              <!-- ${{ product.sale }} -->
              <del class="font-normal text-gray-400">
                $00.00
                <!-- ${{ product.price }} -->
              </del>
            </p>
            <div class="flex my-6">
              <input
                type="number"
                class="w-10 border border-gray-200 mr-5 text-center"
                value="1"
              />
              <button class="bs-button">Add to cart</button>
            </div>

            <div
              class="flex border-b border-gray-200 justify-between text-sm pb-3 mb-8"
            >
              <p class="flex items-center">
                <img src="~/assets/images/heart.svg" class="w-4 mr-3" alt="" />
                Add to favorite's
              </p>
              <p class="flex items-center">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-4 w-4 mr-3"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M8.684 13.342C8.886 12.938 9 12.482 9 12c0-.482-.114-.938-.316-1.342m0 2.684a3 3 0 110-2.684m0 2.684l6.632 3.316m-6.632-6l6.632-3.316m0 0a3 3 0 105.367-2.684 3 3 0 00-5.367 2.684zm0 9.316a3 3 0 105.368 2.684 3 3 0 00-5.368-2.684z"
                  />
                </svg>
                Share
              </p>
            </div>

            <div class="text-xs leading-loose">
              <p>
                <span class="uppercase text-gray-400 w-20 inline-block"
                  >Sku:</span
                >
                sdgdhsdfsfg
                <!-- {{ product.sku }} -->
              </p>
              <p>
                <span class="uppercase text-gray-400 w-20 inline-block"
                  >category:</span
                >

                <!-- <span v-for="item in product.categories" :key="item.id"
                  ><nuxt-link
                    class="bs-dark-green-color"
                    :to="'category/' + item.name"
                    >{{ item.name }}</nuxt-link
                  ><span class="comma">, </span></span
                > -->
              </p>

              <p>
                <span class="uppercase text-gray-400 w-20 inline-block"
                  >tags:</span
                >

                <!-- <span v-for="item in product.tags" :key="item.id"
                  ><nuxt-link
                    class="bs-dark-green-color"
                    :to="'category/' + item.name"
                    >{{ item.name }}</nuxt-link
                  ><span class="comma">, </span></span
                > -->
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      modal: false,
      product: '',
    }
  },
  methods: {
    modalClose() {
      this.$store.dispatch('product-details-modal/resetModal')
    },
  },
  mounted() {
    this.$store.watch(
      () => {
        return this.$store.getters['product-details-modal/getModal']
      },
      (val) => {
        this.modal = val.modal
        this.product = val.product
      },
      {
        deep: true,
      }
    )
  },
}
</script>

<style></style>
