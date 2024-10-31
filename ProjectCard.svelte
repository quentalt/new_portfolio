<script lang="ts">
    export let title: string;
    export let description: string;
</script>

<div class="bg-white p-4 rounded-lg shadow-md transition duration-300 hover:shadow-lg">
    <h3 class="font-semibold text-lg">{title}</h3>
    <p class="mt-2 text-gray-700">{description}</p>
</div>
