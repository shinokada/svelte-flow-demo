<script>
  import "../app.css";
  import { Navbar } from "@codewithshin/svelte-flow";
</script>

<link
  rel="stylesheet"
  href="https://unpkg.com/@themesberg/flowbite@1.3.0/dist/flowbite.min.css"
/>

<div class="mx-auto p-2">
  <Navbar textsize="lg" />
  <div class="mt-4">
    <slot />
  </div>
</div>
