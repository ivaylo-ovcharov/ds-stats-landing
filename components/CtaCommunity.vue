<template>
  <section>
    <div class="max-w-6xl mx-auto px-4 sm:px-6 relative">
      <div class="pt-12 md:pt-20 border-t border-b border-border-default">
        <div
          class="max-w-3xl mx-auto text-center pb-12 md:pb-16"
          data-aos-id-cta
        >
          <!-- Section header -->
          <h1
            class="h2 mb-4"
            data-aos="fade-up"
            data-aos-anchor="[data-aos-id-cta]"
          >
            Ready to enhance your skills?
          </h1>
          <p
            class="text-xl text-body mb-8"
            data-aos="fade-up"
            data-aos-delay="200"
            data-aos-anchor="[data-aos-id-cta]"
          >
            Get the best practices and learn how to build Vue.js app on
            production level
          </p>

          <!-- CTA button -->
          <div
            class="flex justify-center mb-8"
            data-aos="fade-up"
            data-aos-delay="400"
            data-aos-anchor="[data-aos-id-cta]"
          >
            <a
              class="btn px-4 text-white bg-purple-600 hover:bg-purple-700 w-full mb-4 sm:w-auto sm:mb-0"
              href="https://discord.com/channels/1104304995022667846/1104304995505029122"
              target="_blank"
            >
              <!-- Uploaded to: SVG Repo, www.svgrepo.com, Generator: SVG Repo Mixer Tools -->
              Join Early Access</a
            >
          </div>

          <!-- Check list -->
          <ul
            class="flex flex-wrap justify-center text-lg text-body -mx-2 -my-1"
          >
            <li
              class="flex items-center mx-3 my-1"
              data-aos="fade-up"
              data-aos-delay="600"
              data-aos-anchor="[data-aos-id-cta]"
            >
              <svg
                class="w-3 h-3 fill-current text-green-500 mr-2 shrink-0"
                viewBox="0 0 12 12"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"
                />
              </svg>
              <span>Full Access</span>
            </li>
            <li
              class="flex items-center mx-3 my-1"
              data-aos="fade-up"
              data-aos-delay="800"
              data-aos-anchor="[data-aos-id-cta]"
            >
              <svg
                class="w-3 h-3 fill-current text-green-500 mr-2 shrink-0"
                viewBox="0 0 12 12"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"
                />
              </svg>
              <span>Comunnity</span>
            </li>
            <li
              class="flex items-center mx-3 my-1"
              data-aos="fade-up"
              data-aos-delay="1000"
              data-aos-anchor="[data-aos-id-cta]"
            >
              <svg
                class="w-3 h-3 fill-current text-green-500 mr-2 shrink-0"
                viewBox="0 0 12 12"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"
                />
              </svg>
              <span>Recourses</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>
  
  <script>
export default {
  name: "Cta",
};
</script>