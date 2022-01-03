<script lang="ts">
    import Navigation from "./Navigation.svelte";
    import Jumbotron from "./Jumbotron.svelte";
    import Grids from "./Grids.svelte";
</script>

<div id="main">
    <div id="top">
        <Navigation />
        <Jumbotron />
    </div>
    <div id="bottom">
        <Grids />
    </div>
</div>

<style>
    #top {
        background-image: url("/assets/desktop/image-header.jpg");
        background-size: cover;
        background-position: top right;
    }
</style>
