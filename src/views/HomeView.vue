<template>
  <div class="home px-40">
    <div class="grid grid-cols-2 grid-rows-1 gap-4 items-center">
      <div class="sm:col-span-4 md:col-span-2 lg:col-span-1">
        <div class="profile">
          <div class="image flex justify-center">
            <img
              src="https://ahadsenja.github.io/assets/Portfolio%20Me.png"
              alt="Profile"
            />
          </div>
        </div>
      </div>

      <div class="sm:col-span-4 md:col-span-2 lg:col-span-1 text-gray-800">
        <div class="name mb-4">
          <h1 class="text-left text-3xl">Muhamad Hamdanil</h1>
          <span class="flex justify-start text-gray-400"
            >Frontend Developer</span
          >
        </div>

        <p class="text-left">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Magnam
          cumque, <br />
          impedit laboriosam dicta facere architecto deserunt a unde labore
          nihil <br />
          nesciunt aliquam aliquid voluptatibus dolorem laudantium <br />
          sapiente at earum quidem!
        </p>
        <Button class="flex justify-start" />

        <div class="sosmed flex mt-10">
          <a class="pr-20 hover:text-gray-500" href="#">Twitter</a>
          <a class="pr-20 hover:text-gray-500" href="#">Linkedin</a>
          <a class="pr-20 hover:text-gray-500" href="#">Facebook</a>
          <a class="pr-20 hover:text-gray-500" href="#">Instagram</a>
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
export default class HomeView extends Vue {}
</script>
