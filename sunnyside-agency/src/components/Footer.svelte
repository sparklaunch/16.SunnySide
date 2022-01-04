<div id="footer">
    <a href="/">
        <img src="/assets/logo.svg" alt="Logo" />
    </a>

    <div id="sitemaps">
        <a href="#">About</a>
        <a href="#">Services</a>
        <a href="#">Projects</a>
    </div>
    <div id="social-media-links">
        <a href="#">
            <img src="/assets/icon-facebook.svg" alt="Facebook" />
        </a>
        <a href="#">
            <img src="/assets/icon-instagram.svg" alt="Instagram" />
        </a>
        <a href="#">
            <img src="/assets/icon-twitter.svg" alt="Twitter" />
        </a>
        <a href="#">
            <img src="/assets/icon-pinterest.svg" alt="Pinterest" />
        </a>
    </div>
</div>

<style>
    #footer {
        background-color: rgb(132, 206, 189);
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 50px 0;
    }
    #footer > a > img {
        width: 150px;
        filter: brightness(0);
        display: block;
        margin-bottom: 30px;
    }
    #sitemaps {
        margin-bottom: 60px;
    }
    #sitemaps > a {
        text-decoration: none;
        color: rgb(42, 109, 93);
        font-family: "Barlow", sans-serif;
        transition: color 0.3s;
    }
    #sitemaps > a:hover {
        color: white;
    }
    #sitemaps > a:not(:last-child) {
        margin-right: 30px;
    }
    #social-media-links > a {
        text-decoration: none;
    }
    #social-media-links > a:not(:last-child) {
        margin-right: 20px;
    }
    #social-media-links > a > img {
        transition: filter 0.3s;
    }
    #social-media-links > a:hover > img {
        filter: brightness(10);
    }
</style>
