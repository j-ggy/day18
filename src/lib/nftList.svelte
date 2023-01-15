<script lang="ts">
    import { onMount } from "svelte";

    type NFT = {
        imageURL: string;
        name: string;
    };

    let nfts: NFT[] = [];
    let count =0;

    onMount(() => {
        setInterval(() => {
            count ++;
            nfts.push({
                imageURL: ("image #" + count),
                name: ("NFT #" + count)
            });
            nfts = nfts;
        }, 500);
    });
</script>

<h2>
    {#each nfts as nft}{nft.name} - {nft.imageURL}<br/>{/each}
</h2>
