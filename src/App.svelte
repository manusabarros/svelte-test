<script lang="ts">
    import Router from "../node_modules/svelte-spa-router/Router.svelte";
    import { wrap } from "../node_modules/svelte-spa-router/wrap";
    import Header from "./components/Header.svelte";
    import Footer from "./components/Footer.svelte";
    import RootPage from "./pages/RootPage.svelte";

    const routes = {
        "/home": wrap({
            component: RootPage,
            props: {
                name: "Home",
            },
        }),
        "/about": wrap({
            component: RootPage,
            props: {
                name: "About",
            },
        }),
        "/services": wrap({
            component: RootPage,
            props: {
                name: "Services",
            },
        }),
        "/technologies": wrap({
            component: RootPage,
            props: {
                name: "Technologies",
            },
        }),
        "/contact": wrap({
            component: RootPage,
            props: {
                name: "Contact",
            },
        }),
        "*": wrap({
            component: RootPage,
            props: {
                name: "Home",
            },
        }),
    };
</script>

<Header />
<Router {routes} />
<Footer />
