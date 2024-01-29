<template>
  <carousel ref="slider" :items-to-show="1.91" :breakpoints="breakpoints">
    <slide v-for="slide in 10" :key="slide">
      <div
        class="bg-light-grey p-10 rounded-xl relative min-w-[320px] md:min-w-auto mr-8 xl:mr-14"
      >
        <span></span>
        <div>
          <div></div>
          <p class="mb-2">
            <span class="las la-quote-left text-4xl"></span>
          </p>
          <p class="text-[1.5rem] md:text-[2.8rem] text-brand-black">
            We can trust Mono over 90% of the time which is better than our
            previous provider. This ease & reliability are our favourite things
            about Lithobase.
          </p>
          <p class="text-right">
            <span class="las la-quote-right text-4xl"></span>
          </p>
        </div>
        <br />
      </div>
    </slide>

    <template #addons>
      <navigation />
    </template>
  </carousel>

  <div class="my-16 flex justify-end items-center space-x-6">
    <button @click="prev()">
      <span class="las la-long-arrow-alt-left"></span>
    </button>
    <button @click="next()">
      <span class="las la-long-arrow-alt-right"></span>
    </button>
  </div>
</template>

<script>
// If you are using PurgeCSS, make sure to whitelist the carousel CSS classes
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";

export default {
  components: {
    Carousel,
    Slide,
    Navigation,
  },
  data() {
    return {
      breakpoints: {
        300: {
          itemsToShow: 0.95,
          snapAlign: "center",
        },
        // 610px and up
        610: {
          itemsToShow: 1.71,
          snapAlign: "start",
          wrapAround: true,
        },
        // 768px and up
        768: {
          itemsToShow: 0.91,
          snapAlign: "center",
        },
        // 1024 and up
        1024: {
          itemsToShow: 1.91,
          snapAlign: "start",
        },
      },
    };
  },
  methods: {
    next() {
      this.$refs.slider.next();
    },
    prev() {
      this.$refs.slider.prev();
    },
  },
};
</script>
