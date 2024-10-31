<script lang="ts">
    export let src: string; // URL de l'image de profil
    export let alt: string = "Profile Image";
</script>

<div class="flex justify-center mt-6">
    <img src={src} alt={alt} class="rounded-full w-32 h-32 object-cover shadow-lg" />
</div>
