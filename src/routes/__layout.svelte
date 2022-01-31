<script>
  import "../app.css";
  import { Navbar } from "@codewithshin/svelte-flow";

  let menus = [
    {
      name: "Home",
      link: "/",
    },
    {
      name: "Buttons",
      link: "/buttons",
    },
    {
      name: "Cards",
      link: "/cards",
    },
    {
      name: "List Group",
      link: "/list-group",
    },
    {
      name: "Modals",
      link: "/modals",
    },
    {
      name: "Navbar",
      link: "/navbar",
    },
    {
      name: "Tabs",
      link: "/tabs",
    },
  ];
  let logoSrc = "/images/mkdir-logo.png";
</script>

<svelte:head>
  <link
    rel="stylesheet"
    href="https://unpkg.com/@themesberg/flowbite@1.3.0/dist/flowbite.min.css"
  />
</svelte:head>

<div class="container mx-auto px-8">
  <Navbar {menus} />

  <slot />
</div>
