<script lang="ts">
    import { fade } from "svelte/transition";
    let isMenuOpen: boolean = false;
    const hamburgerClickHandler: () => void = () => {
        isMenuOpen = !isMenuOpen;
    };
</script>

<div id="navigation">
    <div id="navigation-title">
        <a href="/">
            <img src="/assets/logo.svg" alt="Logo" />
        </a>
    </div>
    <div id="navigation-menu-desktop">
        <ul>
            <li>
                <a href="#">About</a>
            </li>
            <li>
                <a href="#">Services</a>
            </li>
            <li>
                <a href="#">Projects</a>
            </li>
        </ul>
        <button>CONTACT</button>
    </div>
    <div id="navigation-menu-mobile">
        <img
            src="/assets/icon-hamburger.svg"
            alt="Hamburger Menu"
            on:click={hamburgerClickHandler}
        />
        {#if isMenuOpen}
            <div id="mobile-menu" transition:fade>
                <div id="mobile-menu-tail" />
                <div id="mobile-menu-container">
                    <a href="#">About</a>
                    <a href="#">Services</a>
                    <a href="#">Projects</a>
                    <button>CONTACT</button>
                </div>
            </div>
        {/if}
    </div>
</div>

<style>
    #navigation {
        display: flex;
        padding: 30px;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 50px;
    }
    #navigation-menu-mobile {
        display: none;
    }
    #navigation-menu-desktop {
        display: flex;
        align-items: center;
    }
    #navigation-menu-desktop > ul {
        list-style: none;
        display: flex;
    }
    #navigation-menu-desktop > ul > li {
        margin-right: 30px;
    }
    #navigation-menu-desktop > ul > li > a {
        text-decoration: none;
        font-family: "Barlow", sans-serif;
        color: white;
        font-size: 15px;
    }
    #navigation-menu-desktop > button {
        background-color: white;
        padding: 15px 25px;
        border: none;
        font-family: "Fraunces", sans-serif;
        border-radius: 30px;
        cursor: pointer;
        transition: background-color 0.3s, color 0.3s;
    }
    #navigation-menu-desktop > button:hover {
        background-color: rgb(99, 202, 251);
        color: white;
    }
    @media all and (max-width: 1440px) {
        #navigation-menu-desktop {
            display: none;
        }
        #navigation-menu-mobile {
            display: block;
            position: relative;
        }
        #navigation-menu-mobile > img {
            cursor: pointer;
        }
        #mobile-menu {
            position: absolute;
            right: 0;
            top: 30px;
            width: calc(100vw - 60px);
        }
        #mobile-menu-tail {
            position: absolute;
            border: 20px solid white;
            width: 0;
            height: 0;
            right: -40px;
            top: 30px;
            border-top-color: transparent;
            border-right-color: transparent;
            border-bottom-color: transparent;
            transform: translate(-50%, -50%) rotate(45deg);
        }
        #mobile-menu-container {
            position: absolute;
            right: 0;
            top: 30px;
            width: 100%;
            background-color: white;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 30px;
        }
        #mobile-menu-container > a {
            text-decoration: none;
            font-family: "Barlow", sans-serif;
            color: rgb(124, 118, 128);
            margin-bottom: 25px;
        }
        #mobile-menu-container > button {
            padding: 15px 30px;
            border: none;
            background-color: rgb(250, 208, 1);
            font-family: "Fraunces", sans-serif;
            border-radius: 30px;
            color: rgb(37, 30, 0);
            cursor: pointer;
        }
    }
</style>
