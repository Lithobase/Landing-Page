<template>
  <div>
    <Container>
      <nav class="bg-white py-2">
        <div class="py-4 flex items-center justify-between">
          <router-link
            to="/"
            class="flex items-center space-x-3 rtl:space-x-reverse"
          >
            <img
              src="@/assets/images/logo.png"
              class="h-8"
              alt="Lithobase Logo"
            />
            <span
              class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"
              >Lithobase</span
            >
          </router-link>

          <div
            class="menu-wrapper flex space-x-3 md:space-x-0 rtl:space-x-reverse"
          >
            <div class="items-center justify-between w-full flex">
              <ul
                class="flex flex-col p-4 md:p-0 mt-4 font-medium border border-gray-100 rounded-lg bg-gray-50 md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700"
              >
                <li>
                  <a
                    href="/"
                    class="block py-2 px-3 rounded md:bg-transparent text-blue-700 md:p-0"
                    >Home</a
                  >
                </li>
                <li class="relative">
                  <a
                    href="#"
                    class="flex flex-nowrap items-center space-x-1 py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0"
                    id="dropdownHoverButton"
                    data-dropdown-toggle="dropdownHover"
                    data-dropdown-trigger="hover"
                    ><span>Products</span>
                    <span class="las la-angle-down"></span>
                  </a>

                  <!-- Dropdown menu -->
                  <div
                    id="dropdownHover"
                    class="z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700"
                  >
                    <ul
                      class="py-2 text-sm text-gray-700 dark:text-gray-200"
                      aria-labelledby="dropdownHoverButton"
                    >
                      <li>
                        <a
                          href="/products/PpinaBox"
                          class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                          >Payment Processor
                        </a>
                      </li>
                      <li>
                        <a
                          href="/products/mifos"
                          class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                          >Lithobase Core</a
                        >
                      </li>
                      <li>
                        <a
                          href="/products/search-app"
                          class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                          >Payment Device</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li>
                  <a
                    href="/"
                    class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                    >Services</a
                  >
                </li>
                <li>
                  <a
                    href="/docs/overview"
                    class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                    >Developers</a
                  >
                </li>
                <li>
                  <a
                    href="/"
                    class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                    >Contact</a
                  >
                </li>
              </ul>
            </div>
          </div>

          <div class="">
            <button
              class="hidden lg:inline-flex items-center space-x-4 rounded-full px-5 py-2 pr-3 bg-[#f5f5f5]"
            >
              <span class="">See a Demo</span>
              <div
                class="w-[35px] h-[35px] bg-black rounded-full flex justify-center items-center -rotate-45"
              >
                <span
                  class="las la-long-arrow-alt-right text-lg text-white"
                ></span>
              </div>
            </button>

            <button
              class="inline-flex lg:hidden items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200"
              @click="openMenu = !openMenu"
            >
              <span class="sr-only">Open main menu</span>
              <svg
                class="w-5 h-5"
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 17 14"
              >
                <path
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M1 1h15M1 7h15M1 13h15"
                />
              </svg>
            </button>

            <div
              :class="[
                'mobile-menu w-full bg-white border-b border-t fixed top-20 left-0',
                openMenu ? 'block' : 'hidden',
              ]"
            >
              <ul
                class="p-4 font-medium rounded-lg w-full px-[24px] md:px-0 md:w-[82vw] mx-auto"
              >
                <li>
                  <a
                    href="/"
                    class="block py-2 px-3 rounded md:bg-transparent text-blue-700"
                    >Home</a
                  >
                </li>
                <li class="relative">
                  <a
                    class="block py-2 px-3 text-gray-900 rounded md:hover:bg-transparent md:hover:text-blue-700"
                    id="dropdownDefaultButton"
                    data-dropdown-toggle="dropdown"
                    >Products
                    <span class="las la-angle-down"></span>
                  </a>

                  <!-- Dropdown menu -->
                  <div
                    id="dropdown"
                    class="z-20 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700"
                  >
                    <ul
                      class="py-2 text-sm text-gray-700 dark:text-gray-200"
                      aria-labelledby="dropdownHoverButton"
                    >
                      <li>
                        <a
                          href="/products/PpinaBox"
                          class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                          >Payment Processor
                        </a>
                      </li>
                      <li>
                        <a
                          href="/products/mifos"
                          class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                          >Lithobase Core</a
                        >
                      </li>
                      <li>
                        <a
                          href="/products/search-app"
                          class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                          >Payment Device</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li>
                  <a
                    href="/"
                    class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                    >Services</a
                  >
                </li>
                <li>
                  <a
                    href="/docs/overview"
                    class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                    >Developers</a
                  >
                </li>
                <li>
                  <a
                    href="/"
                    class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                    >Contact</a
                  >
                </li>
              </ul>
            </div>
          </div>
        </div>
      </nav>
    </Container>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import Container from "@/components/partials/Container.vue";

const openMenu = ref(false);
</script>

<style lang="scss" scoped>
@media only screen and (max-width: 1024px) {
  .menu-wrapper {
    display: none;
  }
}
</style>
