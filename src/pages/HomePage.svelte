<script lang="ts">
    import { location, replace } from "../../node_modules/svelte-spa-router/Router.svelte";
    import Home from "../components/Home.svelte";

    if ($location !== "/home") replace("/home");
</script>

<h1>Home Page</h1>
<Home />
