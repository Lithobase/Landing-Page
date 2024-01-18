<template>
  <div class="bg-black">
    <Container class="py-16">
      <div class="text-center py-16">
        <h1
          class="text-white text-[2.5rem] md:text-[4rem] font-semibold mb-4 md:mb-0"
        >
          Start building with Lithobase
        </h1>
        <p class="text-white mb-16 text-[18px] md:text-[25px]">
          Access high-quality financial data and start processing
          <br class="hidden md:inline-block" />
          payments directly from bank accounts in minutes.
        </p>
        <div
          class="flex items-center flex-wrap space-x-1 md:space-x-8 justify-center"
        >
          <button
            class="inline-flex items-center space-x-4 rounded-full px-6 py-4 bg-brand-primary mb-3 md:mb-0"
          >
            <span class="text-white">Start now for free</span>
            <div
              class="w-[35px] h-[35px] bg-white rounded-full flex justify-center items-center -rotate-45"
            >
              <span class="las la-long-arrow-alt-right"></span>
            </div>
          </button>

          <button
            class="inline-flex items-center space-x-4 rounded-full px-6 py-4 bg-gray-500 mb-3 md:mb-0"
          >
            <span class="text-white">Start now for free</span>
            <div
              class="w-[35px] h-[35px] bg-white rounded-full flex justify-center items-center -rotate-45"
            >
              <span
                class="las la-long-arrow-alt-right text-lg text-black"
              ></span>
            </div>
          </button>
        </div>
      </div>

      <div class="my-10 border border-gray-600 w-full h-[1px]"></div>

      <div class="py-16">
        <div class="grid grid-cols-2 md:grid-cols-4 gap-6 md:gap-0">
          <div class="text-white">
            <h4 class="text-gray-400 font-medium mb-4 text-[16px]">Products</h4>
            <ul>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px] font-medium"
                  >Connect</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >QwickSearch</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >Ppina Box</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >Connect</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >QwickSearch</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white">Ppina Box</router-link>
              </li>
            </ul>
          </div>
          <div class="text-white">
            <h4 class="text-gray-400 font-medium mb-4 text-[16px]">
              Resources
            </h4>
            <ul>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px] font-medium"
                  >Connect</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >QwickSearch</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >Ppina Box</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >Connect</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >QwickSearch</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white">Ppina Box</router-link>
              </li>
            </ul>
          </div>
          <div class="text-white">
            <h4 class="text-gray-400 font-medium mb-4 text-[16px]">Company</h4>
            <ul>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px] font-medium"
                  >Connect</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >QwickSearch</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >Ppina Box</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >Connect</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >QwickSearch</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white">Ppina Box</router-link>
              </li>
            </ul>
          </div>
          <div class="text-white">
            <h4 class="text-gray-400 font-medium mb-4 text-[16px]">Legal</h4>
            <ul>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px] font-medium"
                  >Connect</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >QwickSearch</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >Ppina Box</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >Connect</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white text-[14px]"
                  >QwickSearch</router-link
                >
              </li>
              <li class="mb-3">
                <router-link to="/" class="text-white">Ppina Box</router-link>
              </li>
            </ul>
          </div>
        </div>
      </div>

      <div class="mt-10 mb-8 border border-gray-600 w-full h-[1px]"></div>

      <div class="md:flex items-center justify-between text-white space-x-6">
        <div class="flex items-center space-x-2 mb-4 md:mb-0">
          <img
            src="@/assets/images/logo.png"
            class="h-8"
            alt="Lithobase Logo"
          />
          <p>&copy; Lithobase technologies Limited</p>
        </div>

        <div class="flex items-center space-x-6">
          <div class="inline-flex items-center">
            <span class="lab la-twitter text-lg mr-2"></span>
            <span>Twitter</span>
          </div>
          <div class="inline-flex items-center">
            <span class="lab la-linkedin text-lg mr-2"></span>
            <span>LinkedIn</span>
          </div>
        </div>
      </div>
    </Container>
  </div>
</template>

<script setup lang="ts">
import Container from "./Container.vue";
</script>
