<template>
  <section>
    <div class="max-w-6xl mx-auto px-4 sm:px-6">
      <div class="py-12 md:py-20 border-gray-800">
        <!-- Items -->
        <div class="grid gap-20" data-aos-id-features-home>
          <!-- Item -->
          <div class="md:grid md:grid-cols-12 md:gap-6 items-center">
            <!-- Image -->
            <div
              class="max-w-xl md:max-w-none md:w-full mx-auto md:col-span-5 lg:col-span-6 mb-8 md:mb-0 md:order-1"
              data-aos="fade-up"
              data-aos-anchor="[data-aos-id-features-home]"
            >
              <div class="relative">
                <img
                  class="md:max-w-none"
                  src="/course/project.png"
                  width="540"
                  height="520"
                  alt="Features illustration"
                />
                <a href="https://swapi-dusky.vercel.app/" target="_blank">
                  <svg
                    class="hidden md:block absolute inset-0 max-w-full mx-auto md:max-w-none h-auto"
                    width="300"
                    height="300"
                    viewBox="0 0 540 520"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <g class="fill-current text-purple-600">
                      <circle class="pulse" cx="270" cy="260" r="64" />
                      <circle class="pulse pulse-1" cx="270" cy="260" r="64" />
                      <circle class="pulse pulse-2" cx="270" cy="260" r="64" />
                      <circle class="pulse pulse-3" cx="270" cy="260" r="64" />
                    </g>
                  </svg>
                </a>
              </div>
            </div>
            <!-- Content -->
            <div
              class="max-w-xl md:max-w-none md:w-full mx-auto md:col-span-7 lg:col-span-6"
              data-aos="fade-right"
              data-aos-anchor="[data-aos-id-features-home]"
            >
              <div class="md:pr-4 lg:pr-12 xl:pr-16">
                <div
                  class="font-architects-daughter text-xl text-purple-600 mb-2"
                >
                  Project Showcase
                </div>
                <h3 class="h3 mb-3">Discover the Impressive Outcome</h3>
                <p class="text-xl text-body mb-4">
                  By the end of this Vue.js Mastery Course, you'll have
                  developed a complete, production-ready application,
                  demonstrating your newfound skills and expertise.
                </p>
                <!-- <ul
                    class="flex flex-wrap text-lg text-body -mx-2 -my-1 mb-2"
                  >
                    <li class="flex items-center mx-2 my-1">
                      <svg
                        class="w-3 h-3 fill-current text-green-500 mr-2 shrink-0"
                        viewBox="0 0 12 12"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <path
                          d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"
                        />
                      </svg>
                      <span>Design system</span>
                    </li>
                    <li class="flex items-center mx-2 my-1">
                      <svg
                        class="w-3 h-3 fill-current text-green-500 mr-2 shrink-0"
                        viewBox="0 0 12 12"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <path
                          d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"
                        />
                      </svg>
                      <span>Theming</span>
                    </li>
                    <li class="flex items-center mx-2 my-1">
                      <svg
                        class="w-3 h-3 fill-current text-green-500 mr-2 shrink-0"
                        viewBox="0 0 12 12"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <path
                          d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"
                        />
                      </svg>
                      <span>Data Loaders</span>
                    </li>
                  </ul> -->
                <!-- <a
                    class="text-purple-600 hover:text-gray-200 transition duration-150 text-lg ease-in-out"
                    href="https://swapi-dusky.vercel.app/"
                    target="_blank"
                    >Checkout the project</a
                  > -->

                <a
                  class="btn text-white bg-purple-600 hover:bg-purple-700 group"
                  href="https://swapi-dusky.vercel.app/"
                  target="_blank"
                >
                  Checkout the project
                  <span
                    class="tracking-normal text-purple-300 group-hover:translate-x-0.5 transition-transform duration-150 ease-in-out ml-1"
                    >-&gt;</span
                  >
                </a>
                <!-- <div class="flex items-start mt-8">
                    <img class="rounded-full shrink-0 mr-4" src="../images/features-avatar.jpg" width="40" height="40" alt="Features avatar" />
                    <div>
                      <blockquote class="text-body italic m-0 mb-3">"Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing".</blockquote>
                      <div class="text-gray-700 font-medium">
                        <cite class="text-gray-200 not-italic">— Anastasia Dan</cite> - <a class="text-purple-600 hover:text-gray-200 transition duration-150 ease-in-out" href="#0">UX Board</a>
                      </div>
                    </div>
                  </div> -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
  
  <script>
export default {
  name: "FeaturesHome",
};
</script>