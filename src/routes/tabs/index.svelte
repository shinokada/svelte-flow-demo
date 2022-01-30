<script>
  import { List } from "@codewithshin/svelte-flow";

  let lists = [
    {
      title: "Default Tabs",
      link: "/tabs/default-tabs",
    },
    {
      title: "Interactive Tabs",
      link: "/tabs/interactive-tabs",
    },
    {
      title: "Multiple interactive",
      link: "/tabs/multiple-interactive-tabs",
    },
    {
      title: "Pill Tabs",
      link: "/tabs/pilltabs",
    },
  ];
</script>

<div class="container mx-auto p-8">
  <List {lists} />
</div>
