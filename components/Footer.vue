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
  </div>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<style></style>
