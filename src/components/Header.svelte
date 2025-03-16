<script>
  let navbar = [
    { name: 'Home', icon: 'fa-solid fa-house', href: '/' },
    {
      name: 'Notifications',
      icon: 'fa-regular fa-bell',
      href: '/notifications',
    },
    { name: 'Bookmarks', icon: 'fa-regular fa-bookmark', href: '/bookmarks' },
    { name: 'Profile', icon: 'fa-regular fa-user', href: '/profile' },
  ]
</script>

<header class="w-64 h-screen">
  <div
    class="fixed flex flex-col justify-between w-64 h-screen pr-3 overflow-y-auto border-r border-gray-200"
  >
    <a class="flex justify-start my-3" href="/" aria-labelledby="logo">
      <img src="./images/logo.svg" class="h-13" alt="logo" />
    </a>

    <nav class="mt-5">
      <div class="flex flex-col">
        {#each navbar as item}
          <a
            class="flex items-center justify-start mb-8 transition duration-200 ease-in-out"
            href={item.href}
            aria-labelledby="nav"
          >
            <i
              class="text-3xl {item.icon} w-8 h-8 flex items-center text-center justify-center"
            ></i>
            <!-- Set a fixed width here (e.g., 24px) -->
            <span class="ml-4 font-bold text-md">{item.name}</span>
          </a>
        {/each}
      </div>
    </nav>

    <div
      class="flex flex-row justify-between p-2 py-5 mx-auto mt-auto mb-5 transition ease-in-out rounded-full cursor-pointer w-14 xl:w-full bg-complementary hover:bg-primary duration-350"
    >
      <div class="flex flex-row">
        <div class="flex flex-col ml-2 xl:block">
          <h1 class="text-xl font-semibold text-black">Log-in</h1>
        </div>
      </div>
    </div>
  </div>
</header>
