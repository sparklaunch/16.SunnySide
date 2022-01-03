<script lang="ts">
    import Navigation from "./Navigation.svelte";
    import Jumbotron from "./Jumbotron.svelte";
</script>

<div id="main">
    <Navigation />
    <Jumbotron />
</div>

<style>
    #main {
        background-image: url("/assets/desktop/image-header.jpg");
        background-size: cover;
        background-position: top right;
    }
</style>
