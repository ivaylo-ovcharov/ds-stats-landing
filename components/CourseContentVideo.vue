<script setup lang="ts">
const props = defineProps({
  videoId: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    default: "",
  },
  description: {
    type: String,
    default: "x",
  },
});
</script>
<template>
  <section class="relative">
    <div class="max-w-6xl mx-auto px-4 sm:px-6">
      <div class="pb-12 md:pt-20 md:pb-20">
        <div class="max-w-3xl mx-auto">
          <article>
            <header class="mb-8">
              <!-- Title and excerpt -->
              <div class="text-center md:text-left">
                <h1 class="h1 mb-4" data-aos="fade-up">
                  {{ title }}
                </h1>
                <p
                  class="text-xl text-body"
                  data-aos="fade-up"
                  data-aos-delay="200"
                >
                  {{ description }}
                </p>
              </div>
            </header>
            <WistiaPlayer :videoId="videoId" class="mx-auto md:max-w-none" />
          </article>

          <slot />
        </div>
      </div>
    </div>
  </section>
</template>