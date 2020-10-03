<script lang="ts">
    import HomePage from "./HomePage.svelte";
    import AboutPage from "./AboutPage.svelte";
    import ServicesPage from "./ServicesPage.svelte";
    import TechnologiesPage from "./TechnologiesPage.svelte";
    import ContactPage from "./ContactPage.svelte";

    export let name = "";
    document.title = name;
</script>

{#if name === 'Home'}
    <HomePage />
{:else if name === 'About'}
    <AboutPage />
{:else if name === 'Services'}
    <ServicesPage />
{:else if name === 'Technologies'}
    <TechnologiesPage />
{:else if name === 'Contact'}
    <ContactPage />
{:else}
    <HomePage />
{/if}
