<!-- Please remove this file from your project -->
<template>
  <!-- component -->
  <div
    class="
      h-screen
      w-full
      flex
      justify-center
      items-center
    "
  >
    <div
      class="
        bg-image
        w-full
        sm:w-1/2
        md:w-9/12
        lg:w-1/2
        mx-3
        md:mx-5
        lg:mx-0
        shadow-md
        flex flex-col
        md:flex-row
        items-center
        rounded
        z-10
        overflow-hidden
        bg-center bg-cover bg-blue-600
      "
    >
      <div
        class="
          w-full
          md:w-1/2
          flex flex-col
          justify-center
          items-center
          bg-opacity-25 bg-blue-600
          backdrop
        "
      >
        <h1 class="text-3xl md:text-4xl font-extrabold text-white my-2 md:my-0">
          Facericci
        </h1>
        <p class="mb-2 text-white hidden md:block font-mono">
          your social network
        </p>
      </div>
      <div
        class="
          w-full
          md:w-1/2
          flex flex-col
          items-center
          bg-white
          py-5
          md:py-8
          px-4
        "
      >
        <h3 class="mb-4 font-bold text-3xl flex items-center text-blue-500">
          LOGIN
        </h3>
        <form
          action="#"
          class="px-3 flex flex-col justify-center items-center w-full gap-3"
        >
          <input
            type="email"
            placeholder="email.."
            class="
              px-4
              py-2
              w-full
              rounded
              border border-gray-300
              shadow-sm
              text-base
              placeholder-gray-500 placeholder-opacity-50
              focus:outline-none focus:border-blue-500
            "
          />
          <input
            type="password"
            placeholder="password.."
            class="
              px-4
              py-2
              w-full
              rounded
              border border-gray-300
              shadow-sm
              text-base
              placeholder-gray-500 placeholder-opacity-50
              focus:outline-none focus:border-blue-500
            "
          />
          <nuxt-link to="/feed">
          <button
            class="
              flex
              justify-center
              items-center
              bg-blue-500
              hover:bg-blue-600
              text-white
              focus:outline-none focus:ring
              rounded
              px-3
              py-1
            "
          >
          
            <p class="ml-1 text-lg">Login</p>
          </button>
          </nuxt-link>
        </form>
        <p class="text-gray-700 text-sm mt-2">
          don't have an account?
          <a
            href="#"
            class="
              text-green-500
              hover:text-green-600
              mt-3
              focus:outline-none
              font-bold
              underline
            "
          >
            register
          </a>
        </p>
      </div>
    </div>
  </div>
</template>

<style>

body{
  background-color: #15202b;
}

.bg-image {
  background-image: url(https://images3.alphacoders.com/575/thumb-1920-575608.jpg);
}
.backdrop {
  backdrop-filter: blur(2px);
}
</style>
