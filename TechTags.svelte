<script lang="ts">
    import { Badge } from 'flowbite-svelte';
    export let tags: string[]; // Tableau de technologies à afficher en tags
</script>

<div class="flex flex-wrap justify-center space-x-2 mt-4">
    {#each tags as tag}
        <Badge>{tag}</Badge>
    {/each}
</div>
