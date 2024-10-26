<script>
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import Header from "../components/Header.svelte";
  import MobileHeader from "../components/MobileHeader.svelte";

  import { openModal } from "../store";

  let y;
  $: outerHeight = 0;

  function reroute(href) {
    $openModal = false;
    window.location.href = href;
  }
</script>

{#if $openModal}
  <MobileHeader />
{/if}

{#if y > outerHeight}
  <div
    class="bg-white fixed top-0 left-0 w-full flex flex-col z-20 px-4 fadeIn"
  >
    <Header />
  </div>
{/if}
<slot />
<Footer />
<svelte:window bind:scrollY={y} bind:outerHeight />
<!-- header
hero
product description
user reviews
faq
conversion-
footer -->
