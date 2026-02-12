<script lang="ts">
  import { IconSortAscending, IconSortDescending } from "@tabler/icons-svelte";
  import { sort } from "../stores/sort.svelte";
</script>

<!-- @component
Table of contents for easy navigation.
 -->
<div class="flex flex-row gap-1.5 items-center" id="toc">
  <div class="tooltip tooltip-right">
    <div class="tooltip-content">
      {#if sort.ascending}
        Showing newest first
      {:else}
        Showing oldest first
      {/if}
    </div>
    <button
      onclick={() => {
        sort.ascending = !sort.ascending;
      }}
      aria-label="button"
      class="btn btn-sm btn-square bg-gray-300 shadow-sm"
    >
      {#if sort.ascending}
        <IconSortAscending />
      {:else}
        <IconSortDescending />
      {/if}
    </button>
  </div>
</div>
