<template>
  <div class="w-full">
    <div
      class="services flex justify-center items-center flex-col py-12 px-8 w-full lg:w-3/4 mx-auto"
    >
      <div class="flex justify-center flex-col items-center lg:flex-row">
        <h2 class="services-title text-[#3D4D62] font-bold lg:w-full pr-3">
          We offer end-to-end customs services with fast, accurate and compliant
          customs in multiple countries
        </h2>
        <BaseButton class="min-w-max mt-6 lg:mt-0 hidden lg:block"
          >Get in touch</BaseButton
        >
      </div>
      <div class="w-full lg:hidden">
        <div class="carousel-container">
          <transition-group class="carousel">
            <div
              v-for="slide in slides"
              class="slide flex flex-col"
              :key="slide.id"
            >
              <i :class="slide.iconUrl" class="text-[#01a4b7] w-8 h-8 mb-2"></i>
              <h4 class="title text-[#3D4D62] text-xl font-bold mb-2">
                {{ slide.title }}
              </h4>
              <p
                class="description description text-[#3D4D62] text-base font-medium"
              >
                {{ slide.description }}
              </p>
            </div>
          </transition-group>
        </div>
      </div>
      <div
        class="hidden lg:grid grid-cols-1 lg:grid-cols-3 mt-14 gap-16 w-full"
      >
        <div class="flex flex-col justify-between items-start">
          <i class="fa fa-clock text-[#01a4b7] w-8 h-8 mb-2"></i>
          <h4 class="title text-[#3D4D62] text-xl font-bold mb-2">
            Fast and accurate
          </h4>
          <p class="description text-[#3D4D62] text-base font-medium">
            We offer you a full-service offering with fast and accurate customs
            in multiple countries.
          </p>
        </div>
        <div class="lg:flex flex-col justify-between items-start hidden">
          <i class="fa fa-file-text text-[#01a4b7] w-8 h-8 mb-2"></i>
          <h4 class="title text-[#3D4D62] text-xl font-bold mb-2">
            Strict compliance
          </h4>
          <p class="description text-[#3D4D62] text-base font-medium">
            We make sure you are compliant with regulations to mitigate
            customs-related risk and exposure.
          </p>
        </div>
        <div class="lg:flex flex-col justify-between items-start hidden">
          <i class="fa fa-user-circle text-[#01a4b7] w-8 h-8 mb-2"></i>
          <h4 class="title text-[#3D4D62] text-xl font-bold mb-2">
            Qualified professionals
          </h4>
          <p class="description text-[#3D4D62] text-base font-medium">
            Our highly skilled professionals offer customs expert advice to
            optimise your duty management and help you save costs.
          </p>
        </div>
        <div class="lg:flex flex-col justify-between items-start hidden">
          <i class="fa fa-hourglass-end text-[#01a4b7] w-8 h-8 mb-2"></i>
          <h4 class="title text-[#3D4D62] text-xl font-bold mb-2">
            Online and real-time control
          </h4>
          <p class="description text-[#3D4D62] text-base font-medium">
            Real-time compliance and finance dashboards to manage your customer
            portfolio.
          </p>
        </div>
        <div class="lg:flex flex-col justify-between items-start hidden">
          <i class="fa fa-flag text-[#01a4b7] w-8 h-8 mb-2"></i>
          <h4 class="title text-[#3D4D62] text-xl font-bold mb-2">
            EU-wide-coverage
          </h4>
          <p class="description text-[#3D4D62] text-base font-medium">
            We have offices in 5 European countries, but thanks to our network
            of trusted partners we have EU-wide coverage.
          </p>
        </div>
        <div class="lg:flex flex-col justify-between items-start hidden">
          <i class="fa fa-lightbulb text-[#01a4b7] w-8 h-8 mb-2"></i>
          <h4 class="title text-[#3D4D62] text-xl font-bold mb-2">
            Innovation and digitalisation
          </h4>
          <p class="description text-[#3D4D62] text-base font-medium">
            We use advanced IT-tools for customs declaration and customs data
            exchange.
          </p>
        </div>
      </div>
      <div class="lg:hidden flex justify-between items-center w-full my-5">
        <nav class="carousel flex gap-4 mt-4">
          <span
            v-for="n in 6"
            :key="n"
            class="carousel-item bg-[#CCCCCC] rounded-full"
            type="radio"
            name="carousel-dots"
          ></span>
        </nav>
        <div class="flex">
          <button @click="previous">
            <i class="fa fa-chevron-left text-[gray] mr-3"></i>
          </button>
          <button @click="next">
            <i class="fa fa-chevron-right text-[#01a4b7]" @click="next"></i>
          </button>
        </div>
      </div>
      <BaseButton class="w-full lg:min-w-max mt-6 lg:mt-0 block lg:hidden"
        >Get in touch</BaseButton
      >
    </div>
    <img src="../assets/Gruppe maskieren 2@2x.png" alt="" />
  </div>
</template>

<script>
import BaseButton from "./Base/BaseButton.vue";

export default {
  name: "PageServices",
  components: { BaseButton },
  data() {
    return {
      slides: [
        {
          id: 1,
          iconUrl: `fa fa-clock`,
          title: "Fast and accurate",
          description:
            "We offer you a full-service offering with fast and accurate customs in multiple countries.",
        },
        {
          id: 2,
          iconUrl: "fa fa-file-text",
          title: "Strict compliance",
          description:
            "We make sure you are compliant with regulations to mitigate customs-related risk and exposure.",
        },
        {
          id: 3,
          iconUrl: " fa fa-user-circle",
          title: "Qualified professionals",
          description:
            "Our highly skilled professionals offer customs expert advice to optimise your duty management and help you save costs.",
        },
        {
          id: 4,
          iconUrl: "fa fa-hourglass-end",
          title: "Online and real-time control",
          description:
            "Real-time compliance and finance dashboards to manage your customer portfolio.",
        },
        {
          id: 5,
          iconUrl: "fa fa-flag",
          title: "EU-wide coverage",
          description:
            "We have offices in 5 European countries, but thanks to our network of trusted partners we have EU-wide coverage.",
        },
        {
          id: 6,
          iconUrl: "fa fa-lightbulb",
          title: "Innovation and digitalisation",
          description:
            "We use advanced IT-tools for customs declaration and customs data exchange.",
        },
      ],
    };
  },
  methods: {
    next() {
      console.log("next");
      const first = this.slides.shift();
      this.slides = this.slides.concat(first);
    },
    previous() {
      console.log("prev");
      const last = this.slides.pop();
      this.slides = [last].concat(this.slides);
    },
  },
};
</script>

<style lang="css" scoped>
.carousel {
  display: flex;
  justify-content: space-between;
  align-items: center;
  overflow: hidden;
}

.slide {
  flex: 0 0 100%;
  display: flex;
  justify-content: center;
  padding: 50px 0;
  transition: all 0.3s;
  margin: 20px 0;
}

.carousel-controls__button {
  cursor: pointer;
  border: 0;
  border-radius: 3px;
  padding: 5px 10px;
  font-size: 18px;
}
.services .services-title {
  font-size: 30px;
  max-width: 100%;
  position: relative;
}
.services .services-title::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -32px;
  background-color: #01a4b7;
  height: 3px;
  width: 50px;
  border-radius: 20px;
  margin-bottom: 8px;
}
nav.carousel .carousel-item {
  width: 7px;
  height: 7px;
}

@media only screen and (min-width: 1024px) {
  .services {
    padding: 64px 100px;
  }
  .services .title {
    max-width: 70%;
  }
}
</style>
