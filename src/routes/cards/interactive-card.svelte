<script>
  import { InteractiveCard } from "svelte-flow";
  let dropdownLinks = [
    {
      href: "/#",
      name: "Edit",
    },
    {
      href: "/#",
      name: "About",
    },
    {
      href: "/#",
      name: "Profile",
    },
  ];
  let img = {
    src: "/images/profile-picture-3.jpeg",
    alt: "Suzan Boil",
  };
  let img2 = {
    src: "/images/profile-picture-1.jpeg",
    alt: "John Doe",
  };
  let img3 = {
    src: "/images/profile-picture-2.jpeg",
    alt: "Jane Doe",
  };
  let img4 = {
    src: "/images/profile-picture-4.jpeg",
    alt: "James Smith",
  };
  let header = "Lorem ipsum";
  let content = "Proin efficitur purus felis.";
  let link1 = { href: "/dummy-pages/profile", title: "Profile" };
  let link2 = { href: "/dummy-pages/about", title: "About" };
</script>

<div class=" mx-auto p-8">
  <div class="flex-auto p-4">
    <InteractiveCard {dropdownLinks} {img} {header} {content} {link1} {link2} />
  </div>
  <div class="flex-auto p-4">
    <InteractiveCard
      {dropdownLinks}
      {img}
      {header}
      {content}
      {link1}
      {link2}
      btnColor1="purple"
    />
  </div>
  <div class="flex-auto p-4">
    <InteractiveCard
      {dropdownLinks}
      {img}
      {header}
      {content}
      {link1}
      {link2}
      btnColor1="green"
    />
  </div>
  <div class="flex-auto p-4">
    <InteractiveCard
      {dropdownLinks}
      {img}
      {header}
      {content}
      {link1}
      btnColor1="red"
    />
  </div>
</div>
<div class="flex flex-wrap mx-auto p-8 justify-center">
  <div class="flex-auto p-4">
    <InteractiveCard {dropdownLinks} {img} {header} {content} {link2} />
  </div>
  <div class="flex-auto p-4">
    <InteractiveCard {dropdownLinks} {img} {header} {content} />
  </div>
</div>
