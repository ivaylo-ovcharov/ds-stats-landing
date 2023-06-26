<template>
  <section class="relative">
    <div class="max-w-6xl mx-auto px-4 sm:px-6">
      <div class="pt-32 pb-12 md:pt-40 md:pb-20">
        <!-- Page header -->
        <div class="max-w-3xl pb-12 md:pb-20 text-center md:text-left">
          <h1 class="h1" data-aos="fade-up">
            Eleveate your Frontend skills with this Course
          </h1>
        </div>

        <div class="pb-12 md:pb-20">
          <article
            class="max-w-sm mx-auto md:max-w-none grid md:grid-cols-2 gap-6 md:gap-8 lg:gap-12 xl:gap-16 items-center"
          >
            <div class="relative block group">
              <div
                class="absolute inset-0 bg-gray-800 hidden md:block transform md:translate-y-2 md:translate-x-4 xl:translate-y-4 xl:translate-x-8 group-hover:translate-x-0 group-hover:translate-y-0 transition duration-700 ease-out pointer-events-none"
                aria-hidden="true"
              ></div>
              <router-link to="/courses/build-app-swapi-and-vue">
                <figure
                  class="relative h-0 pb-9/16 md:pb-3/4 lg:pb-9/16 overflow-hidden transform md:-translate-y-2 xl:-translate-y-4 group-hover:translate-x-0 group-hover:translate-y-0 transition duration-700 ease-out"
                >
                  <img
                    class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                    src="/course/swapi-banner.png"
                    alt="Blog post 01"
                  />
                </figure>
              </router-link>
            </div>

            <div data-aos="fade-left" data-aos-delay="200">
              <header>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1"></ul>
                </div>
                <h3 class="h3 text-2xl lg:text-3xl mb-2">
                  Design and Build web app with Swapi and Vue.js
                </h3>
              </header>
              <p class="text-lg text-body grow">
                Enhance your learning experience with our carefully curated
                resources designed to complement the Vue.js Mastery Course.
                Access Figma files, in-depth guides, and reusable code snippets.
              </p>
              <router-link
                class="btn mt-4 px-4 text-white bg-purple-600 hover:bg-purple-700 w-full mb-4 sm:w-auto sm:mb-0"
                to="/courses/build-app-swapi-and-vue"
              >
                Learn more</router-link
              >
            </div>
          </article>
        </div>

        <div class="max-w-sm mx-auto md:max-w-none">
          <h4
            class="h4 pb-6 mb-10 border-b border-border-default"
            data-aos="fade-up"
          >
            Upcoming courses
          </h4>

          <div
            class="grid gap-12 md:grid-cols-3 md:gap-x-6 md:gap-y-8 items-start"
          >
            <article class="flex flex-col h-full">
              <header>
                <a to="/blog-post" class="block mb-6">
                  <figure
                    class="relative h-0 pb-9/16 overflow-hidden rounded-sm"
                  >
                    <img
                      class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                      src="/course/coursedesignsystem.png"
                      width="352"
                      height="198"
                      alt="News 01"
                    />
                  </figure>
                </a>

                <h3 class="h4 mb-2">
                  <a
                    to="/blog-post"
                    class="hover:text-gray-100 transition duration-150 ease-in-out"
                    >Build Your Own Design System - Figma & Vue</a
                  >
                </h3>
              </header>
              <p class="text-lg text-body grow">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </p>
              <router-link
                class="btn mt-4 px-4 text-white bg-purple-600 hover:bg-purple-700 w-full mb-4 sm:w-auto sm:mb-0"
                to="/courses/build-your-own-design-system"
              >
                Learn more</router-link
              >
            </article>
            <article class="flex flex-col h-full">
              <header>
                <a to="/blog-post" class="block mb-6">
                  <figure
                    class="relative h-0 pb-9/16 overflow-hidden rounded-sm"
                  >
                    <img
                      class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                      src="/course/Landing.png"
                      width="352"
                      height="198"
                      alt="News 01"
                    />
                  </figure>
                </a>

                <h3 class="h4 mb-2">
                  <a
                    class="hover:text-gray-100 transition duration-150 ease-in-out"
                    >Create landing pages with Tailwind snippets
                  </a>
                </h3>
              </header>
              <p class="text-lg text-body grow">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </p>
            </article>
            <article class="flex flex-col h-full">
              <header>
                <a to="/blog-post" class="block mb-6">
                  <figure
                    class="relative h-0 pb-9/16 overflow-hidden rounded-sm"
                  >
                    <img
                      class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                      src="/course/Poker.png"
                      width="352"
                      height="198"
                      alt="News 01"
                    />
                  </figure>
                </a>

                <h3 class="h4 mb-2">
                  <a
                    to="/blog-post"
                    class="hover:text-gray-100 transition duration-150 ease-in-out"
                    >Build a Planning App from Design to Deploy</a
                  >
                </h3>
              </header>
              <p class="text-lg text-body grow">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </p>
            </article>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BlogList",
};
</script>