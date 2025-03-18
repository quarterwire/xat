<script lang="ts">
  import '../app.css'
  import '@fortawesome/fontawesome-free/css/all.min.css'
  import Header from '../components/Header.svelte'
  import Right from '../components/Right.svelte'
  import Main from '../components/Main.svelte'
  let { children } = $props()
</script>

<div class="container h-screen mx-auto">
  <div class="flex flex-row justify-center">
    <div><Header /></div>
    <div><Main /></div>
    <div><Right /></div>
  </div>
</div>
