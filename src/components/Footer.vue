<template>
  <div
    class="
      flex
      justify-center
      items-center
      bottom-0
      absolute
      text-sm
      w-full
      pb-2
    "
  >
    <span>
      Copyright &copy; 2022
      <a href="https://www.instagram.com/ahadsenja"
        ><strong>ahadsenja</strong></a
      >. All rights reserved
    </span>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({})
export default class Footer extends Vue {}
</script>