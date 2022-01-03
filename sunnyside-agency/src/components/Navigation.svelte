<div id="navigation">
    <div id="navigation-title">
        <img src="/assets/logo.svg" alt="Logo" />
    </div>
    <div id="navigation-menu">
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
</div>

<style>
    #navigation {
        display: flex;
        padding: 30px;
        justify-content: space-between;
        align-items: center;
    }
    #navigation-menu {
        display: flex;
        align-items: center;
    }
    #navigation-menu > ul {
        list-style: none;
        display: flex;
    }
    #navigation-menu > ul > li {
        margin-right: 30px;
    }
    #navigation-menu > ul > li > a {
        text-decoration: none;
        font-family: "Barlow", sans-serif;
        color: white;
        font-size: 15px;
    }
    #navigation-menu > button {
        background-color: white;
        padding: 15px 25px;
        border: none;
        font-family: "Fraunces", sans-serif;
        border-radius: 30px;
        cursor: pointer;
    }
</style>
