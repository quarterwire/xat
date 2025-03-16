<script>
  import Right from './Right.svelte'
  import Xeet from './Xeet.svelte'
</script>

<main class="h-screen w-160">
  <div
    class="sticky top-0 flex items-center justify-between gap-5 px-4 py-3 border-b border-gray-200"
  >
    <h2
      class="flex flex-col items-center font-bold text-center text-gray-800 font-sm"
    >
      Home
    </h2>
    <i class="fa-solid fa-paw text-2xl text-primary"></i>
  </div>
  <Xeet message="Buna!!!!" />
  <Xeet message="Hawwwooo!!!" />
</main>
