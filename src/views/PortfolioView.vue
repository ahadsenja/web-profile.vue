<template>
  <div class="grid grid-cols-3 grid-rows-1 gap-6 px-40">
    <div
      class="sm:col-span-3 md:col-span-2 lg:col-span-1 mb-8"
      v-for="portfolio in portfolios"
      v-bind:key="portfolio"
    >
      <div class="project">
        <div class="image flex justify-center">
          <img src="https://picsum.photos/420/240" alt="Profile" />
        </div>

        <div class="content mt-4 justify-center">
          <h1 class="flex justify-center text-3xl mb-3">
            {{ portfolio.title }}
          </h1>
          <p class="text-gray-400">
            {{ portfolio.description }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Button from "@/components/Button.vue";

@Options({
  components: {
    Button,
  },
})
export default class PortfolioView extends Vue {
  portfolios: object[] = [
    {
      id: 1,
      title: "Portfolio 1",
      description:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam cumque, impedit laboriosam dicta facere architecto deserunt",
    },
    {
      id: 2,
      title: "Portfolio 2",
      description:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam cumque, impedit laboriosam dicta facere architecto deserunt",
    },
    {
      id: 3,
      title: "Portfolio 3",
      description:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam cumque, impedit laboriosam dicta facere architecto deserunt",
    },
    {
      id: 4,
      title: "Portfolio 4",
      description:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam cumque, impedit laboriosam dicta facere architecto deserunt",
    },
    {
      id: 5,
      title: "Portfolio 5",
      description:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam cumque, impedit laboriosam dicta facere architecto deserunt",
    },
    {
      id: 6,
      title: "Portfolio 6",
      description:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam cumque, impedit laboriosam dicta facere architecto deserunt",
    },
  ];
}
</script>