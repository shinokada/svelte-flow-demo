<script>
  import "../app.css";
  import "@themesberg/flowbite/dist/flowbite.css";
  import { Navbar } from "@codewithshin/svelte-flow";
</script>

<div class="mx-auto p-2">
  <Navbar textsize="lg" />
  <div class="mt-4">
    <slot />
  </div>
</div>
