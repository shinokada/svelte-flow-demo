<script>
  import "../app.css";
  import "flowbite/dist/flowbite.css";
  import { Navbar } from "@codewithshin/svelte-flow";
</script>

<div class="mx-auto px-4">
  <Navbar textsize="lg" />
  <div class="mt-8">
    <slot />
  </div>
</div>
