<script lang="ts">
    import Router from '../node_modules/svelte-spa-router/Router.svelte';
    import HomePage from './pages/HomePage.svelte';
    import AboutPage from './pages/AboutPage.svelte';
    import ServicesPage from './pages/ServicesPage.svelte';
    import TechnologiesPage from './pages/TechnologiesPage.svelte';
    import ContactPage from './pages/ContactPage.svelte';

    const routes = {
        '/': HomePage,
        '/about': AboutPage,
        '/services': ServicesPage,
        '/technologies': TechnologiesPage,
        '/contact': ContactPage,
    };
</script>

<style type="text/scss">
</style>

<Router {routes} />
