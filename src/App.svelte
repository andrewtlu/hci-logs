<script>
  import ControlGroup from "./components/ControlGroup.svelte";
  import Info from "./components/Info.svelte";
  import P1 from "./components/P1.svelte";
  import P2 from "./components/P2.svelte";
  import P3 from "./components/P3.svelte";
  import { sort } from "./stores/sort.svelte";

  let posts = [P1, P2, P3];
</script>

<svelte:head>
  <title>HCI Project Team Portfolio</title>
</svelte:head>

<main
  class="w-screen min-h-screen bg-base-100 flex justify-center items-center flex-col"
>
  <!-- "nav" -->
  <header></header>

  <div
    class="px-4 w-full md:w-187.5 bg-transparent flex justify-center gap-8 flex-col"
  >
    <!-- title -->
    <div class="flex flex-col gap-2">
      <h1 class="text-4xl font-bold pb-1 mt-15">🍰 GrubAble</h1>
      <div class="divider"></div>
      <Info />
      <div class="divider"></div>
      <ControlGroup />
    </div>

    <!-- p1, p2, ... -->
    <div
      class="flex gap-8"
      class:flex-col-reverse={sort.ascending}
      class:flex-col={!sort.ascending}
    >
      {#each posts as Post, idx (idx)}
        <Post />
      {/each}
    </div>
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
