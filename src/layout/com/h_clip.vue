<template>
  <div
    class="p-3"
    @click="fold"
  >
    <svg
      class="w-6"
      :class="{ 'transform rotate-90': !State.menu_fold }"
      version="1.0"
      xmlns="http://www.w3.org/2000/svg"
      id="Layer_1"
      data-name="Layer 1"
      viewBox="0 0 24 24"
    >
      <g
        id="_01_align_center"
        data-name="01 align center"
      >
        <path
          d="M6.983,24.007A7,7,0,0,1,2.02,12.054l10.6-10.585a5.008,5.008,0,0,1,7.091,7.075L9.11,19.128a3.083,3.083,0,0,1-4.254,0,3,3,0,0,1,0-4.245L14.75,5.007l1.418,1.415L6.274,16.3a1,1,0,0,0,0,1.414,1.027,1.027,0,0,0,1.418,0L18.3,7.129a3.005,3.005,0,1,0-4.255-4.245L3.438,13.468a5.008,5.008,0,0,0,7.09,7.076l12.021-12,1.418,1.415-12.021,12A7,7,0,0,1,6.983,24.007Z"
        />
      </g>
    </svg>
  </div>
</template>

<script setup lang="ts">
import { useStateStore } from "@/store/useStateStore";
const State = useStateStore();

const fold = () => {
  State.menu_fold = !State.menu_fold;
};
</script>

<style scoped lang="scss"></style>
