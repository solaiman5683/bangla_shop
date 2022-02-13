<template>
  <div class="p-6">
    <vue-slick-carousel :arrows="false" :dots="true">
      <div class="bg-green rounded-2xl px-32 pt-8">
        <div class="flex items-center">
          <div class="w-2/3">
            <p class="text-green-500 font-medium text-3xl mb-4">
              Save up 30% off
            </p>
            <h2 class="text-dark-500 font-bold text-7xl leading-tight mb-6">
              Bengal Vegetable <br />
              farm Organic 100%
            </h2>
            <p class="mb-6 w-3/4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae
              aperiam nostrum possimus repellendus ad facere quas aspernatur
              necessitatibus!
            </p>
            <button class="btn">Shop Now</button>
          </div>
          <div class="w-1/3">
            <img src="~/assets/images/hero.png" alt="" />
          </div>
        </div>
      </div>
      <div class="bg-green rounded-2xl px-32 pt-8">
        <div class="flex items-center">
          <div class="w-2/3">
            <p class="text-green-500 font-medium text-3xl mb-4">
              Save up 50% off
            </p>
            <h2 class="text-dark-500 font-bold text-7xl leading-tight mb-6">
              Bengal Vegetable <br />
              farm Organic 100%
            </h2>
            <p class="mb-6 w-3/4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae
              aperiam nostrum possimus repellendus ad facere quas aspernatur
              necessitatibus!
            </p>
            <button class="btn">Shop Now</button>
          </div>
          <div class="w-1/3">
            <img src="~/assets/images/hero.png" alt="" />
          </div>
        </div>
      </div>
    </vue-slick-carousel>

    <div class="container">
      <!-- Category Section -->
      <section class="py-12">
        <h3 class="text-xl font-medium mb-6">Search by Category</h3>
        <div class="flex items-center mb-8">
          <div
            style="height: 4px"
            class="w-1/12 bg-green-500 rounded-full"
          ></div>
          <div style="height: 2px" class="w-11/12 bg-gray-200"></div>
        </div>

        <!-- Catagories -->
        <vue-slick-carousel
          class="category-carousel"
          v-bind="categoryCarouselSettings"
        >
          <div>
            <div
              class="flex items-center flex-col p-4 bg-gray-200 rounded-xl m-2"
            >
              <img src="~/assets/images/category1.png" alt="" />
              <h4 class="text-xl font-medium mb-2">Groceries</h4>
            </div>
          </div>
          <div>
            <div
              class="flex items-center flex-col p-4 bg-gray-200 rounded-xl m-2"
            >
              <img src="~/assets/images/category2.png" alt="" />
              <h4 class="text-xl font-medium mb-2">Fish</h4>
            </div>
          </div>
          <div>
            <div
              class="flex items-center flex-col p-4 bg-green-100 rounded-xl m-2"
            >
              <img src="~/assets/images/category3.png" alt="" />
              <h4 class="text-xl font-medium mb-2">Meat</h4>
            </div>
          </div>
          <div>
            <div
              class="flex items-center flex-col p-4 bg-gray-200 rounded-xl m-2"
            >
              <img src="~/assets/images/category4.png" alt="" />
              <h4 class="text-xl font-medium mb-2">Vegetables</h4>
            </div>
          </div>
          <div>
            <div
              class="flex items-center flex-col p-4 bg-gray-200 rounded-xl m-2"
            >
              <img src="~/assets/images/category5.png" alt="" />
              <h4 class="text-xl font-medium mb-2">Fruits</h4>
            </div>
          </div>
          <div>
            <div
              class="flex items-center flex-col p-4 bg-gray-200 rounded-xl m-2"
            >
              <img src="~/assets/images/category6.png" alt="" />
              <h4 class="text-xl font-medium mb-2">Ice Cream</h4>
            </div>
          </div>
          <div>
            <div
              class="flex items-center flex-col p-4 bg-gray-200 rounded-xl m-2"
            >
              <img src="~/assets/images/category1.png" alt="" />
              <h4 class="text-xl font-medium mb-2">Vegetables</h4>
            </div>
          </div>

          <template #prevArrow>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M15 19l-7-7 7-7"
              />
            </svg>
          </template>
          <template #nextArrow>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 5l7 7-7 7"
              /></svg
          ></template>
        </vue-slick-carousel>
      </section>

      <section class="py-8">
        <div class="flex gap-6">
          <div class="w-1/2">
            <img src="~/assets/images/promo1.png" alt="" />
          </div>
          <div class="w-1/2">
            <img src="~/assets/images/promo2.png" alt="" />
          </div>
        </div>
      </section>

      <!-- Featured Products -->
      <section class="py-12">
        <h3 class="text-xl font-medium mb-6">Deals of the Week</h3>
        <div class="flex items-center mb-8">
          <div
            style="height: 4px"
            class="w-1/12 bg-green-500 rounded-full"
          ></div>
          <div style="height: 2px" class="w-11/12 bg-gray-200"></div>
        </div>

        <!-- Products -->
        <vue-slick-carousel
          class="category-carousel"
          v-bind="productCarouselSettings"
        >
          <SingleProduct />
          <SingleProduct />
          <SingleProduct />
          <SingleProduct />
          <SingleProduct />
          <SingleProduct />
          <SingleProduct />
          <SingleProduct />

          <template #prevArrow>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M15 19l-7-7 7-7"
              />
            </svg>
          </template>
          <template #nextArrow>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 5l7 7-7 7"
              /></svg
          ></template>
        </vue-slick-carousel>
      </section>

      <!-- Brands Section -->
      <section class="py-8">
        <h3 class="text-xl font-medium mb-6">Popular Brands</h3>
        <div class="flex items-center mb-8">
          <div
            style="height: 4px"
            class="w-1/12 bg-green-500 rounded-full"
          ></div>
          <div style="height: 2px" class="w-11/12 bg-gray-200"></div>
        </div>

        <!-- Brands -->
        <vue-slick-carousel
          class="category-carousel mb-16 text-center"
          v-bind="categoryCarouselSettings"
        >
          <div>
            <div class="flex items-center justify-center h-32">
              <img src="~/assets/images/brand1.png" alt="" />
            </div>
          </div>
          <div>
            <div class="flex items-center justify-center h-32">
              <img src="~/assets/images/brand2.png" alt="" />
            </div>
          </div>
          <div>
            <div class="flex items-center justify-center h-32">
              <img src="~/assets/images/brand3.png" alt="" />
            </div>
          </div>
          <div>
            <div class="flex items-center justify-center h-32">
              <img src="~/assets/images/brand4.png" alt="" />
            </div>
          </div>
          <div>
            <div class="flex items-center justify-center h-32">
              <img src="~/assets/images/brand5.png" alt="" />
            </div>
          </div>
          <div>
            <div class="flex items-center justify-center h-32">
              <img src="~/assets/images/brand6.png" alt="" />
            </div>
          </div>
          <div>
            <div class="flex items-center justify-center h-32">
              <img src="~/assets/images/brand3.png" alt="" />
            </div>
          </div>

          <template #prevArrow>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M15 19l-7-7 7-7"
              />
            </svg>
          </template>
          <template #nextArrow>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 5l7 7-7 7"
              /></svg
          ></template>
        </vue-slick-carousel>
      </section>
      <!-- Collections -->
      <section class="py-8">
        <div class="flex gap-4">
          <div class="w-1/3 p-4 rounded-xl flex bg-yellow-100">
            <div class="flex py-4 pl-6 flex-col justify-around h-full w-1/2">
              <h3 class="text-3xl">Fresh Fruits Collection</h3>
              <nuxt-link
                to="/"
                class="h-12 w-12 rounded-full shadow bg-white flex items-center justify-center"
                ><svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M13 7l5 5m0 0l-5 5m5-5H6"
                  /></svg
              ></nuxt-link>
            </div>
            <div class="w-1/2">
              <img width="100%" src="~/assets/images/fruits.png" alt="" />
            </div>
          </div>

          <div class="w-1/3 p-4 rounded-xl flex bg-green-200">
            <div class="flex py-4 pl-6 flex-col justify-around h-full w-1/2">
              <h3 class="text-3xl">Vegetable Collection</h3>
              <nuxt-link
                to="/"
                class="h-12 w-12 rounded-full shadow bg-white flex items-center justify-center"
                ><svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M13 7l5 5m0 0l-5 5m5-5H6"
                  /></svg
              ></nuxt-link>
            </div>
            <div class="w-1/2">
              <img width="100%" src="~/assets/images/vegetable.png" alt="" />
            </div>
          </div>

          <div class="w-1/3 p-4 rounded-xl flex bg-yellow-200">
            <div class="flex py-4 pl-6 flex-col justify-around h-full w-1/2">
              <h3 class="text-3xl">Grocery Item</h3>
              <nuxt-link
                to="/"
                class="h-12 w-12 rounded-full shadow bg-white flex items-center justify-center"
                ><svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M13 7l5 5m0 0l-5 5m5-5H6"
                  /></svg
              ></nuxt-link>
            </div>
            <div class="w-1/2">
              <img width="100%" src="~/assets/images/grocery.png" alt="" />
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import SingleProduct from '~/components/SingleProduct.vue'
export default {
  name: 'IndexPage',
  data() {
    return {
      categoryCarouselSettings: {
        slidesToShow: 6,
        slidesToScroll: 1,
      },
      productCarouselSettings: {
        slidesToShow: 5,
        slidesToScroll: 1,
      },
    }
  },
}
</script>
