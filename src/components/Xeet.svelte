<script>
  export let message
</script>

<div
  class="border-b border-gray-200 hover:bg-gray-100 cursor-pointer transition duration-350 ease-in-out pb-4 border-l border-r"
>
  <div class="flex flex-shrink-0 p-4 pb-0">
    <a href="/" aria-labelledby="tweet" class="flex-shrink-0 group block">
      <div class="flex items-start">
        <div>
          <img
            alt="profile"
            class="inline-block h-9 w-9 rounded-full"
            src="https://thumbs.dreamstime.com/b/cute-cat-portrait-square-photo-beautiful-white-closeup-105311158.jpg"
          />
        </div>
        <div class="ml-3">
          <p
            class="flex items-center text-[15px] leading-6 font-semibold text-gray-800"
          >
            Cat Facts
            <span
              class="ml-1 text-sm leading-5 font-medium transition ease-in-out text-gray-400 duration-150"
            >
              @xatfactsdaily . Nov 7
            </span>
          </p>
        </div>
      </div>
    </a>
  </div>
  <div class="pl-16 pr-5">
    <p class="text-base width-auto font-medium text-gray-800 flex-shrink">
      {message}
    </p>
    <div class="flex my-3 mr-2 rounded-2xl border border-gray-400">
      <img
        class="rounded-2xl w-full"
        src="https://www.dailypaws.com/thmb/ZHs0nxwPjwixC4YkqyRcO9DB2bg=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/striped-cat-playing-flower-552781357-2000-f8b1f07162594830bdba8a24e2268ad6.jpg"
        alt=""
      />
    </div>
    <div class="flex gap-44">
      <div
        class="flex items-center text-gray-800 text-xs transition duration-350 ease-in-out hover:text-primary"
      >
        <i class="fa-regular fa-message w-5 h-5 text-2xl mr-2"></i>
        <p class="text-md">13.4k</p>
      </div>
      <div
        class="flex items-center text-gray-800 text-xs transition duration-350 ease-in-out hover:text-red-500"
      >
        <i class="fa-regular fa-heart w-5 h-5 text-2xl mr-2"></i>
        <p class="text-md">13.4k</p>
      </div>
      <div
        class="flex items-center text-gray-800 text-center text-xs transition duration-350 ease-in-out hover:text-yellow-500"
      >
        <i class="fa-regular fa-bookmark w-5 h-5 text-2xl mr-2"></i>
        <p class="text-md">13.4k</p>
      </div>
    </div>
  </div>
</div>
