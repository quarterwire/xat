<script lang="ts">
  import { onMount } from 'svelte'
  import Xeet from './Xeet.svelte'

  let catFacts: string[] = []

  async function getCatFact() {
    const requests = Array.from({ length: 6 }, () =>
      fetch(`https://catfact.ninja/fact`).then((res) => res.json())
    )
    const facts = await Promise.all(requests)
    catFacts = facts.map((fact) => fact.fact) // Ensure reactivity by reassigning the array
  }

  onMount(() => {
    getCatFact()
  })
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

  {#each catFacts as catFact}
    <Xeet message={catFact} />
  {/each}
</main>
