<template>
  <div>
    <Container>
      <nav class="bg-white py-2">
        <div
          class="w-full px-[24px] md:px-0 md:w-[82vw] mx-auto flex flex-wrap items-center justify-between p-4"
        >
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
            class="flex md:order-2 space-x-3 md:space-x-0 rtl:space-x-reverse"
          >
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
              data-collapse-toggle="navbar-sticky"
              type="button"
              class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
              aria-controls="navbar-sticky"
              aria-expanded="false"
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
          </div>
          <div
            class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1"
            id="navbar-sticky"
          >
            <ul
              class="flex flex-col p-4 md:p-0 mt-4 font-medium border border-gray-100 rounded-lg bg-gray-50 md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700"
            >
              <li>
                <a
                  href="#"
                  class="block py-2 px-3 text-white bg-blue-700 rounded md:bg-transparent md:text-blue-700 md:p-0 md:dark:text-blue-500"
                  aria-current="page"
                  >Home</a
                >
              </li>
              <li class="relative">
                <a
                  href="#"
                  class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                  id="dropdownHoverButton"
                  data-dropdown-toggle="dropdownHover"
                  data-dropdown-trigger="hover"
                  >Products
                  <span class="las la-angle-down"></span>
                  </a
                >

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
                      <router-link to="/products/ppinabox"
                        href="#"
                        class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                        >Payment Processor </router-link
                      >
                    </li>
                    <li>
                      <router-link to="/products/mifos"
                        class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                        >Lithobase Core</router-link
                      >
                    </li>
                    <li>
                      <router-link to="/products/search-app"
                        class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                        >Payment Device</router-link
                      >
                    </li>
                  </ul>
                </div>
              </li>
              <li>
                <a
                  href="#"
                  class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                  >Services</a
                >
              </li>
              <li>
                <router-link to="/docs/overview"
                  href="#"
                  class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                  >Developers</router-link
                >
              </li>
              <li>
                <a
                  href="#"
                  class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
                  >Contact</a
                >
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </Container>
  </div>
</template>

<script setup lang="ts">
import Container from "@/components/partials/Container.vue";
</script>
