<template>
  <div class="lg:grid lg:grid-cols-2 lg:gap-4 lg:mr-5">
    <content-placeholders
      :rounded="true"
      v-for="item in items"
      :key="item"
      class="mb-6"
    >
      <content-placeholders-img style="height: 12rem" />
      <!-- <content-placeholders-heading :img="true" /> -->
      <!-- <content-placeholders-heading /> -->
      <content-placeholders-text />
    </content-placeholders>
  </div>
</template>

<script>
export default {
  props: ["items"],
};
</script>
