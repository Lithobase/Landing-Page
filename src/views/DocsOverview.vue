<template>
  <div>
    <Container>
      <div class="py-16 text-center">
        <div class="mb-16">
          <small
            class="inline-block mb-2 bg-[#F5F5F5] p-2 px-4 font-semibold rounded-lg"
            >Lithobase for developers</small
          >
          <h1
            class="font-semibold text-[2.5rem] md:text-[3.6rem] leading-[120%] mb-6"
          >
            A complete API suite to build <br class="hidden md:inline-block" />
            amazing payments experiences
          </h1>
          <p class="text-[18px] leading-[180%] mb-8">
            Lithobase is literally the most secured way to integrate
            <br class="hidden md:inline-block" />
            payments into your applications.
          </p>

          <div class="flex justify-center items-center space-x-5 mb-10">
            <a
              :href="docsUrl"
              target="_blank"
              class="inline-flex items-center space-x-4 rounded-full px-6 pr-2 py-2 bg-brand-primary"
            >
              <span class="text-white">Explore Docs</span>
              <div
                class="w-[35px] h-[35px] bg-white rounded-full flex justify-center items-center -rotate-45"
              >
                <span class="las la-long-arrow-alt-right"></span>
              </div>
            </a>
          </div>
        </div>
      </div>
    </Container>
  </div>

  <div class="bg-[#F5F5F5] py-16">
    <Container>
      <div class="py-16">
        <div class="mb-16">
          <h1
            class="font-semibold text-[2rem] md:text-[3.2rem] leading-[120%] mb-6"
          >
            Build awesome products
          </h1>
          <p class="text-[22px] text-gray-500 leading-[180%]">
            What can you build with Lithobase? Here’s how our APIs
            <br class="hidden md:inline-block" />
            come together to bring ideas to life.
          </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mb-8">
          <div class="p-10 rounded-xl bg-white">
            <h2 class="mb-3 text-[25px] font-semibold">Transactions API</h2>
            <p class="text-[18px] leading-[170%]">
              Get paid by your customers in multiple currencies
            </p>

            <p
              class="text-[16px] leading-[180%] flex space-x-2 items-center mt-4"
            >
              <span
                class="text-brand-primary las la-chevron-circle-right text-2xl mt-2"
              ></span>
              <a
              :href="docsUrl"
                class="font-semibold text-brand-primary inline-block mt-1"
                >Learn more</a
              >
            </p>
          </div>

          <div class="p-10 rounded-xl bg-white">
            <h2 class="mb-3 text-[25px] font-semibold">Transfer API</h2>
            <p class="text-[18px] leading-[170%]">
              Automatically transfer money directly to your customers' bank
              accounts.
            </p>

            <p
              class="text-[16px] leading-[180%] flex space-x-2 items-center mt-4"
            >
              <span
                class="text-brand-primary las la-chevron-circle-right text-2xl mt-2"
              ></span>
              <a
              :href="docsUrl"
                class="font-semibold text-brand-primary inline-block mt-1"
                >Learn more</a
              >
            </p>
          </div>

          <div class="p-10 rounded-xl bg-white">
            <h2 class="mb-3 text-[25px] font-semibold">Charge Authorization</h2>
            <p class="text-[18px] leading-[170%]">
              Debit a customer and get a unique token you can use for future
              charges.
            </p>

            <p
              class="text-[16px] leading-[180%] flex space-x-2 items-center mt-4"
            >
              <span
                class="text-brand-primary las la-chevron-circle-right text-2xl mt-2"
              ></span>
              <a
              :href="docsUrl"
                class="font-semibold text-brand-primary inline-block mt-1"
                >Learn more</a
              >
            </p>
          </div>

          <div class="p-10 rounded-xl bg-white">
            <h2 class="mb-3 text-[25px] font-semibold">Accounts API</h2>
            <p class="text-[18px] leading-[170%]">
              Verify if the bank account details provided by customers are
              correct.
            </p>

            <p
              class="text-[16px] leading-[180%] flex space-x-2 items-center mt-4"
            >
              <span
                class="text-brand-primary las la-chevron-circle-right text-2xl mt-2"
              ></span>
              <a
              :href="docsUrl"
                class="font-semibold text-brand-primary inline-block mt-1"
                >Learn more</a
              >
            </p>
          </div>
        </div>
      </div>
    </Container>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import Container from "@/components/partials/Container.vue";

const docsUrl = ref("https://lithobase.gitbook.io/lithobase/");
</script>
