<script lang="ts">
  import svelteLogo from './assets/svelte.svg'
  import AlertUser from './lib/alertUser.svelte';
  import Name from './lib/name.svelte'
  import NftList from './lib/nftList.svelte';
</script>

<main>
  <div>
    <p>{name}</p>
    <a href="https://vitejs.dev" target="_blank" rel="noreferrer"> 
      <img src="/vite.svg" class="logo" alt="Vite Logo" />
    </a>
    <a href="https://svelte.dev" target="_blank" rel="noreferrer"> 
      <img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
    </a>
  </div>
  <h1>Vite + Svelte</h1>

  <div class="card">
    <Name></Name>
    <AlertUser></AlertUser>
    <NftList></NftList>
  </div>

</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
</style>