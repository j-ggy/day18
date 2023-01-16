<script lang="ts">
    import { onMount } from "svelte";

    type NFT = {
        imageURL: string;
        name: string;
    };

    let nfts: NFT[] = [];

    onMount(() => {
        setInterval(() => {
            nfts.push({
                imageURL: ("image #" + nfts.length),
                name: ("NFT #" + nfts.length)
            });
            nfts = nfts;
        }, 500);
    });
</script>

<h2>
    {#each nfts as nft}{nft.name} - {nft.imageURL}<br/>{/each}
</h2>
