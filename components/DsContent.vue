<script>
export default {
  name: "News",
  data() {
    return {
      courses: [
        {
          name: "Design System - Tokens",
          img: "/course/ds-tokens-cover.png",
          link: "/courses/design-system/tokens",
          description:
            "Learn the language that both designers and developers understand",
        },
        {
          name: "Tokens - Color Mapping",
          img: "/course/ds-colors.png",
          link: "/courses/design-system/tokens-colors",
          description:
            "Learn how to build managable color system together with theming",
        },
        {
          name: "Tokens - Typography",
          img: "/course/ds-typography.png",
          link: "/courses/design-system/tokens-typography",
          description:
            "Build managable typography system (Still working on that)",
        },
        {
          name: "Design system - Components",
          img: "/course/comingsoon.png",
          description:
            "We will create a method that will allow us to fetch data with a single line of code, we will also include caching",
        },
        {
          name: "Componentds - Button",
          img: "/course/comingsoon.png",
          description:
            "Once we have all building blocks done we will put the peaces together and create our DataTable component",
        },
        {
          name: "Components - Table",
          img: "/course/comingsoon.png",
          description:
            "Final UI/UX alignments and preparation for release, some details that most developers miss",
        },
      ],
    };
  },
};
</script>

<template>
  <section>
    <div class="max-w-6xl mx-auto px-4 sm:px-6">
      <div class="py-12 md:py-20">
        <div class="max-w-sm mx-auto md:max-w-none">
          <div
            class="grid gap-12 md:grid-cols-3 md:gap-x-6 md:gap-y-8 items-start"
          >
            <article
              v-for="course in courses"
              :key="course"
              class="flex flex-col h-full"
            >
              <header>
                <router-link :to="course.link || ''" class="block mb-6">
                  <figure
                    class="relative h-0 pb-9/16 overflow-hidden rounded-sm"
                    style="box-shadow: 20px 20px 60px #011321"
                  >
                    <img
                      class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                      :src="course.img"
                      width="352"
                      height="198"
                      alt="News 01"
                    />
                  </figure>
                </router-link>
                <h3 class="h4 mb-2">
                  <router-link
                    :to="course.link || ''"
                    class="hover:text-gray-100 transition duration-150 ease-in-out"
                    >{{ course.name }}</router-link
                  >
                </h3>
                <p class="text-lg text-body grow">
                  {{ course.description }}
                </p>
              </header>
            </article>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

