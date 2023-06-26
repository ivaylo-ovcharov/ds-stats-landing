<script setup>
const items = ref([
  {
    section: true,
    name: "Tokens",
  },
  {
    name: "Design System - Tokens (5:10)",
    link: "/courses/design-system/tokens",
  },
  {
    name: "Tokens - Color Mapping (8:01)",
    link: "/courses/design-system/tokens-colors",
  },
  // {
  //   name: "Tokens - Typography Composition",
  //   link: "/courses/design-system/tokens-typography",
  // },
  {
    section: true,
    name: "Components",
  },
  // {
  //   name: "Components - Create Button with variants",
  //   link: "/courses/design-system/components-button",
  // },
  // {
  //   name: "Components - Create Table with Composition",
  //   link: "/courses/design-system/components-table",
  // },
  {
    name: "Features - Build Invite User Dialog with Paste Design System (4:23)",
    link: "/courses/design-system/invite-user-dialog",
  },
  {
    section: true,
    name: "Project Management",
  },
  {
    name: "Project Management 101 (2:52)",
    link: "/courses/design-system/project-management-basics",
  },
  {
    name: "Break down and Visualize (3:58)",
    link: "/courses/design-system/project-management-101",
  },
  {
    name: "Design System Stats - Visualize Automation (1:04)",
    link: "/courses/design-system/project-management-automator",
  },
]);

const route = useRoute();

const prevPage = computed(() => {
  const currentPage = items.value.find((item) => item.link === route.path);
  const currentPageIndex = items.value.indexOf(currentPage);

  return items.value[currentPageIndex - 1] || false;
});

const nextPage = computed(() => {
  const currentPage = items.value.find((item) => item.link === route.path);
  const currentPageIndex = items.value.indexOf(currentPage);

  return items.value[currentPageIndex + 1] || false;
});
</script>
<template>
  <div class="antialiased bg-gray-50 dark:bg-gray-900">
    <nav
      class="bg-surface border-b border-border-default px-4 py-2.5 dark:bg-gray-800 dark:border-gray-700 fixed left-0 right-0 top-0 z-50"
    >
      <div class="flex flex-wrap justify-between items-center">
        <IdButton variant="plain" to="/courses">
          <IconPrev /> Go Back to Courses
        </IdButton>
        <button
          data-drawer-target="drawer-navigation"
          data-drawer-toggle="drawer-navigation"
          aria-controls="drawer-navigation"
          class="p-2 mr-2 text-gray-600 rounded-lg cursor-pointer md:hidden hover:text-gray-900 hover:bg-gray-100 focus:bg-gray-100 dark:focus:bg-gray-700 focus:ring-2 focus:ring-gray-100 dark:focus:ring-gray-700 dark:text-gray-400 dark:hover:bg-gray-700 dark:hover:text-white"
        >
          <svg
            aria-hidden="true"
            class="w-6 h-6"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h6a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
              clip-rule="evenodd"
            ></path>
          </svg>
          <svg
            aria-hidden="true"
            class="hidden w-6 h-6"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
              clip-rule="evenodd"
            ></path>
          </svg>
          <span class="sr-only">Toggle sidebar</span>
        </button>
        <!-- <div class="absolute text-center" style="left: 0; right: 0">
          Design System
        </div> -->
        <div class="hidden md:flex gap-4">
          <IdButton v-if="prevPage" :to="prevPage.link" variant="secondary">
            <IconPrev /> Previous Lesson
          </IdButton>
          <IdButton v-if="nextPage" :to="nextPage.link" variant="secondary">
            Next Lesson
            <IconNext />
          </IdButton>
        </div>
      </div>
    </nav>

    <aside
      class="fixed top-0 left-0 z-40 w-96 h-screen pt-14 transition-transform -translate-x-full bg-surface border-r border-border-default md:translate-x-0 overflow-scroll"
      aria-label="Sidenav"
    >
      <div class="pt-10 pb-2 px-3 h4">Build your own design system</div>
      <div class="py-5 h-full bg-surface dark:bg-gray-800">
        <ul>
          <li v-for="item in items" :key="item">
            <router-link
              v-if="!item.section"
              :to="item.link"
              class="flex items-center px-4 py-3 text-base font-medium text-gray-300 hover:bg-surfacehover"
              :class="
                route.path === item.link && '!bg-purple-600 !bg-opacity-20'
              "
            >
              <div class="w-5 h-5">
                <div
                  v-if="item.completed"
                  class="w-5 h-5 rounded-full border-2 border-purple-600 bg-purple-600 flex justify-center items-center"
                >
                  <IconTick class="w-3 h-3" />
                </div>
                <div
                  v-else
                  class="w-5 h-5 rounded-full border-2 border-purple-600 flex"
                ></div>
              </div>

              <span class="ml-3">{{ item.name }}</span>
            </router-link>
            <div
              class="my-2 ml-5 pb-2 font-semibold border-b border-border-default"
              v-else
            >
              {{ item.name }}
            </div>
          </li>
        </ul>
      </div>
    </aside>

    <main class="p-4 md:ml-64 h-auto pt-20 min-h-screen bg-surface">
      <slot />
    </main>
  </div>
</template>
