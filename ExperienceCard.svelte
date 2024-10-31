<script lang="ts">
    export let title: string;
    export let description: string;
    export let duration: string;
</script>

<div class="bg-white p-4 rounded-lg shadow-md transition duration-300 hover:shadow-lg">
    <h3 class="font-semibold text-lg">{title}</h3>
    <p class="text-sm text-gray-600">{duration}</p>
    <p class="mt-2 text-gray-700">{description}</p>
</div>
