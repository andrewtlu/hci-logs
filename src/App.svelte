<script>
  import ControlGroup from "./components/ControlGroup.svelte";
  import P1 from "./components/P1.svelte";
  import P2 from "./components/P2.svelte";
  import { sort } from "./stores/sort.svelte";

  let posts = $derived.by(() => {
    let p = [P1, P2];
    return sort.ascending ? [...p].reverse() : p;
  });
</script>

<svelte:head>
  <title>HCI Project Team Portfolio</title>
</svelte:head>

<main
  class="w-screen min-h-screen bg-base-100 flex justify-center items-center flex-col"
>
  <!-- "nav" -->
  <header></header>

  <div class="w-187.5 bg-transparent flex justify-center gap-8 flex-col">
    <!-- title -->
    <div class="flex flex-col gap-2">
      <h1 class="text-4xl font-bold pb-1 mt-15">🍰 NutriCare</h1>
      <h2>Sumon Kanti Dey, Andrew Lu, & Julian Lucio Paredes</h2>
      <div class="divider"></div>
      <ControlGroup />
    </div>

    <!-- p1, p2, ... -->
    {#each posts as Post, idx (idx)}
      <Post />
    {/each}
  </div>

  <!-- footer -->
  <footer
    class="footer sm:footer-horizontal footer-center bg-transparent text-neutral-content p-10"
  >
    <a
      href="https://github.com/andrewtlu/hci-logs/"
      class="link link-hover link-primary">GitHub Repository</a
    >
  </footer>
</main>
