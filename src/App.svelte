<svelte:options customElement="global-search" />

<script>
  import searchLogo from "./assets/icons/search.svg";
  import Modal from "./lib/Modal.svelte";
  let showModal = false;
</script>

<div class="searchBox">
  <div class="searchContainer">
    <img src={searchLogo} alt="search-logo" height="20px" width="20px" />
    <button class="btn" on:click={() => (showModal = true)}> Search </button>
  </div>
</div>

<Modal bind:showModal/>