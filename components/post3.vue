<template>
  <!-- component -->
  <!-- This is an example component -->
  <div class="">
    <div
      class="
        flex
        max-w-xl
        my-10
        bg-gray-400
        shadow-md
        rounded-lg
        overflow-hidden
        mx-auto
      "
    >
      <div class="flex items-center w-full">
        <div class="w-full">
          <div class="flex flex-row mt-2 px-2 py-3 mx-3">
            <div class="w-auto h-auto rounded-full border-2 border-pink-500">
              <img
                class="
                  w-12
                  h-12
                  object-cover
                  rounded-full
                  shadow
                  cursor-pointer
                "
                alt="User avatar"
                src="data:image/png;base64,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"
              />
            </div>
            <div class="flex flex-col mb-2 ml-4 mt-1">
              <div class="text-gray-600 text-sm font-semibold">Chess.com</div>
              <div class="flex w-full mt-1">
                <div
                  class="text-blue-700 font-base text-xs mr-1 cursor-pointer"
                >
                  Xadrez
                </div>
                <div class="text-gray-400 font-thin text-xs">
                  • 1 day ago
                </div>
              </div>
            </div>
          </div>
          <div class="border-b border-gray-600"></div>
          <div class="text-gray-400 font-medium text-sm mb-7 mt-6 mx-3 px-2">
            <img
              class="rounded"
              src="https://images.chesscomfiles.com/uploads/v1/news/1015157.28fe2258.668x375o.0afd4dcbd3d8.png"
            />
          </div>
          <div class="text-gray-600 font-semibold text-lg mb-2 mx-3 px-2">
            Campeonato Mundial da FIDE: Nepomniachtchi impressiona sob pressão e
            empata a 1ª partida
          </div>
          <div class="text-gray-500 font-thin text-sm mb-6 mx-3 px-2">
            O campeão mundial, Magnus Carlsen, e o desafiante, Ian
            Nepomniachtchi, começaram o match do Campeonato Mundial da FIDE
            nesta sexta-feira, em Dubai, com um empate. Nepomniachtchi tinha uma
            ligeira vantagem na abertura, mas foi pressionado pouco depois e
            impressionou com um jogo preciso no final. A segunda partida está
            agendada para sábado, às 16h30 em Dubai (09:30 de Brasília, 12:30 de
            Lisboa).
          </div>
          <div class="flex justify-start mb-4 border-t border-gray-600">
            <div class="flex w-full mt-1 pt-2 pl-5">
              <span
                class="
                  bg-white
                  transition
                  ease-out
                  duration-300
                  hover:text-red-500
                  border
                  w-8
                  h-8
                  px-2
                  pt-2
                  text-center
                  rounded-full
                  text-gray-400
                  cursor-pointer
                  mr-2
                "
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  width="14px"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M5 5a2 2 0 012-2h10a2 2 0 012 2v16l-7-3.5L5 21V5z"
                  />
                </svg>
              </span>
              <img
                class="
                  inline-block
                  object-cover
                  w-8
                  h-8
                  text-white
                  border-2 border-white
                  rounded-full
                  shadow-sm
                  cursor-pointer
                "
                src="https://images.unsplash.com/photo-1491528323818-fdd1faba62cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
                alt=""
              />
              <img
                class="
                  inline-block
                  object-cover
                  w-8
                  h-8
                  -ml-2
                  text-white
                  border-2 border-white
                  rounded-full
                  shadow-sm
                  cursor-pointer
                "
                src="https://images.unsplash.com/photo-1550525811-e5869dd03032?ixlib=rb-1.2.1&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
                alt=""
              />
              <img
                class="
                  inline-block
                  object-cover
                  w-8
                  h-8
                  -ml-2
                  text-white
                  border-2 border-white
                  rounded-full
                  shadow-sm
                  cursor-pointer
                "
                src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80"
                alt=""
              />
              <img
                class="
                  inline-block
                  object-cover
                  w-8
                  h-8
                  -ml-2
                  text-white
                  border-2 border-white
                  rounded-full
                  shadow-sm
                  cursor-pointer
                "
                src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
                alt=""
              />
            </div>
            <div class="flex justify-end w-full mt-1 pt-2 pr-5">
              <span
                class="
                  transition
                  ease-out
                  duration-300
                  hover:bg-blue-50
                  bg-blue-100
                  h-8
                  px-2
                  py-2
                  text-center
                  rounded-full
                  text-blue-400
                  cursor-pointer
                  mr-2
                "
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  width="14px"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M8.684 13.342C8.886 12.938 9 12.482 9 12c0-.482-.114-.938-.316-1.342m0 2.684a3 3 0 110-2.684m0 2.684l6.632 3.316m-6.632-6l6.632-3.316m0 0a3 3 0 105.367-2.684 3 3 0 00-5.367 2.684zm0 9.316a3 3 0 105.368 2.684 3 3 0 00-5.368-2.684z"
                  />
                </svg>
              </span>
              <span
                class="
                  transition
                  ease-out
                  duration-300
                  hover:bg-blue-500
                  bg-blue-600
                  h-8
                  px-2
                  py-2
                  text-center
                  rounded-full
                  text-gray-100
                  cursor-pointer
                "
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  width="14px"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4"
                  />
                </svg>
              </span>
            </div>
          </div>
          <div class="flex w-full border-t border-gray-600">
            <div class="mt-3 mx-5 flex flex-row">
              <div
                class="
                  flex
                  text-gray-700
                  font-normal
                  text-sm
                  rounded-md
                  mb-2
                  mr-4
                  items-center
                "
              >
                Comments:
                <div class="ml-1 text-gray-400 font-thin text-ms">20k</div>
              </div>
              <div
                class="
                  flex
                  text-gray-700
                  font-normal
                  text-sm
                  rounded-md
                  mb-2
                  mr-4
                  items-center
                "
              >
                Views:
                <div class="ml-1 text-gray-400 font-thin text-ms">100k</div>
              </div>
            </div>
            <div class="mt-3 mx-5 w-full flex justify-end">
              <div
                class="
                  flex
                  text-gray-700
                  font-normal
                  text-sm
                  rounded-md
                  mb-2
                  mr-4
                  items-center
                "
              >
                Likes:
                <div class="ml-1 text-gray-400 font-thin text-ms">50k</div>
              </div>
            </div>
          </div>
          <div
            class="
              relative
              flex
              items-center
              self-center
              w-full
              max-w-xl
              p-4
              overflow-hidden
              text-gray-600
              focus-within:text-gray-400
            "
          >
            <img
              class="
                w-10
                h-10
                object-cover
                rounded-full
                shadow
                mr-2
                cursor-pointer
              "
              alt="User avatar"
              src="https://pbs.twimg.com/profile_images/1184313670278549504/I3wVVB_E_400x400.jpg"
            />
            <span class="absolute inset-y-0 right-0 flex items-center pr-6">
              <button
                type="submit"
                class="
                  p-1
                  focus:outline-none focus:shadow-none
                  hover:text-blue-500
                "
              >
                <svg
                  class="
                    w-6
                    h-6
                    transition
                    ease-out
                    duration-300
                    hover:text-blue-500
                    text-gray-400
                  "
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M14.828 14.828a4 4 0 01-5.656 0M9 10h.01M15 10h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
                  />
                </svg>
              </button>
            </span>
            <input
              type="search"
              class="
                w-full
                py-2
                pl-4
                pr-10
                text-sm
                bg-gray-100
                border border-transparent
                appearance-none
                rounded-tg
                placeholder-gray-400
                focus:bg-white
                focus:outline-none
                focus:border-blue-500
                focus:text-gray-900
                focus:shadow-outline-blue
              "
              style="border-radius: 25px"
              placeholder="Post a comment..."
              autocomplete="off"
            />
          </div>
        </div>
      </div>
    </div>
    <script
      data-name="BMC-Widget"
      data-cfasync="false"
      src="https://cdnjs.buymeacoffee.com/1.0.0/widget.prod.min.js"
      data-id="matheusgongo"
      data-description="Support me on Buy me a coffee!"
      data-message="Thank you for visiting! :D"
      data-color="#BD5FFF"
      data-position="Right"
      data-x_margin="18"
      data-y_margin="18"
    ></script>
  </div>
</template>

<style scoped>
</style>