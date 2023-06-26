<template>
  <NuxtLink
    activeClass="text-purple-700"
    class="flex items-center px-3 group text-body hover:text-purple-600 transition duration-150 ease-in-out font-semibold cursor-pointer"
    :to="to"
  >
    <span> <slot /></span>
    <svg
      class="w-3 h-3 fill-current shrink-0 ml-2 transition duration-150 ease-in-out transform"
      :class="`opacity-0 group-hover:translate-x-1 group-hover:opacity-100 group-hover:text-purple-600`"
      viewBox="0 0 12 12"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M11.707 5.293L7 .586 5.586 2l3 3H0v2h8.586l-3 3L7 11.414l4.707-4.707a1 1 0 000-1.414z"
      />
    </svg>
  </NuxtLink>
</template>
<script setup>
const props = defineProps({
  to: {
    type: String,
    defaut: "/",
  },
});
</script>