<script lang="ts">
  const alertUser = () => {
    alert('Okay, you like pushing buttons.')
  }
</script>

<button on:click={alertUser}>
  Don't Touch Me!
</button>
