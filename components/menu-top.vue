<template>
  <!-- component -->
  <div class="flex-1 flex flex-col">
    <nav class="px-4 flex justify-between bg-gray-400  h-16 border-b-2">
      <!-- top bar left -->

      <ul class="flex items-center">
        <!-- add button -->
        <li>
          <h1
            class="text-3xl md:text-4xl font-extrabold text-black my-2 md:my-0"
          >
            Facericci
          </h1>
        </li>
      </ul>

      <!-- to bar right  -->
      <ul class="flex items-center">
        <li class="pr-6">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-bell"
          >
            <path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"></path>
            <path d="M13.73 21a2 2 0 0 1-3.46 0"></path>
          </svg>
        </li>
        <li class="h-10 w-10">
          <img
            class="h-full w-full rounded-full mx-auto"
            src="https://pbs.twimg.com/profile_images/1184313670278549504/I3wVVB_E_400x400.jpg"
            alt="profile woman"
          />
        </li>
      </ul>
    </nav>
  </div>
</template>