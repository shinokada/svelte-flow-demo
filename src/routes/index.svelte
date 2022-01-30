<script>
  import { List } from "@codewithshin/svelte-flow";

  let lists = [
    {
      title: "Home",
      link: "/",
    },
    {
      title: "Alerts",
      link: "/alert",
      external: true,
    },
    {
      title: "Cards",
      link: "/cards",
    },
    {
      title: "List Group",
      link: "/list-group/list",
    },
    {
      title: "Modals",
      link: "/modals",
    },
    {
      title: "Tabs",
      link: "/tabs",
      external: true,
    },
  ];
</script>

<div class="container mx-auto p-8">
  <List {lists} />
</div>
