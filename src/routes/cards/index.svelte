<script>
  import { Card } from "svelte-flow";
</script>

<div class="container flex flex-wrap mx-auto mt-8 justify-center">
  <div class="p-4">
    <Card img="/images/cards.png" header="CARD" link="/cards/card" />
  </div>
  <div class="p-4">
    <Card img="/images/cards.png" header="CTA CARD" link="/cards/cta-card" />
  </div>
  <div class="p-4">
    <Card
      img="/images/cards.png"
      header="ECOMMERCE CARD"
      link="/cards/ecommerce-card"
    />
  </div>
  <div class="p-4">
    <Card
      img="/images/cards.png"
      header="INTERACTIVE CARD"
      link="/cards/interactive-card"
    />
  </div>
  <div class="p-4">
    <Card img="/images/cards.png" header="LIST CARD" link="/cards/list-card" />
  </div>
</div>
