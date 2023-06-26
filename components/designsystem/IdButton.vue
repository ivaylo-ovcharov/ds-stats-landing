<script setup>
const props = defineProps({
  variant: {
    type: String,
    default: "primary",
  },
  to: {
    type: String,
    default: "",
  },
});

const types = {
  secondary: "bg-gray-700 hover:bg-gray-800",
  primary: "bg-purple-600 hover:bg-purple-700",
  plain: " px-0 hover:border-b-white py-1",
};
</script>
<template>
  <router-link
    class="btn text-white w-full sm:w-auto px-4 flex gap-2"
    :class="types[variant]"
    :to="to"
  >
    <slot />
  </router-link>
</template>