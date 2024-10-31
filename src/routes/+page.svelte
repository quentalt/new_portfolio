<script>
    import AppBar from "../components/AppBar.svelte";
    import ProjectCard from "../components/ProjectCard.svelte";
    import TechTags from "../components/TechTags.svelte";
    import ExperienceCard from "../components/ExperienceCard.svelte";
    import ProfileImage from "../components/ProfileImage.svelte";

    const techTags = ["TypeScript", "Svelte", "Tailwind CSS", "Node.js"];
    const experiences = [
        { title: "Développeur Full Stack", description: "Développement d'applications...", duration: "2021 - Présent" },
        { title: "Stage en DevOps", description: "Automatisation de CI/CD...", duration: "2020 - 2021" }
    ];
    const projects = [
        { title: "Mon Portfolio", description: "Application web de présentation personnelle..." },
        { title: "Application de suivi de lecture", description: "Gestion des livres et lectures..." }
    ];
</script>

<AppBar />

<section class="text-center mt-20 p-4">
    <h1 class="text-2xl font-bold">Bonjour, je suis Quentin Altieri</h1>
    <p class="mt-2">Développeur Full Stack passionné par le développement web et mobile.</p>
    <ProfileImage src="photo.jpg" alt="Votre Photo" />
    <TechTags tags={techTags} />
</section>

<section class="p-4 mt-8">
    <h2 class="text-xl font-semibold mb-4">Mes Expériences</h2>
    <div class="space-y-4">
        {#each experiences as { title, description, duration }}
            <ExperienceCard {title} {description} {duration} />
        {/each}
    </div>
</section>

<section class="p-4 mt-8">
    <h2 class="text-xl font-semibold mb-4">Mes Projets</h2>
    <div class="space-y-4">
        {#each projects as { title, description }}
            <ProjectCard {title} {description} />
        {/each}
    </div>
</section>

<style lang="postcss">
    :global(html) {
        background-color: theme(colors.gray.100);
    }
</style>