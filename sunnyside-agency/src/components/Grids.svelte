<div id="grids">
    <div id="transform">
        <h3>Transform your brand</h3>
        <p>
            We are a full-service creative agency specializing in helping brands
            grow fast. Engage your clients through compelling visuals that do
            most of the marketing for you.
        </p>
        <div id="transform-link">
            <a href="#">LEARN MORE</a>
            <div id="transform-link-bottom" />
        </div>
    </div>
    <div id="egg">
        <img src="/assets/desktop/image-transform.jpg" alt="Egg" />
    </div>
    <div id="glass">
        <img src="/assets/desktop/image-stand-out.jpg" alt="Glass" />
    </div>
    <div id="standout">
        <h3>Stand out to the right audience</h3>
        <p>
            Using a collaborative formula of designers, researchers,
            photographers, videographers, and copywriters, we'll build and
            extend your brand in digital places.
        </p>
        <div id="standout-link">
            <a href="#">LEARN MORE</a>
            <div id="standout-link-bottom" />
        </div>
    </div>
    <div id="graphic">
        <h3>Graphic Design</h3>
        <p>
            Great design makes you memorable. We deliver artwork that
            underscores your brand message and captures potential clients'
            attention.
        </p>
    </div>
    <div id="photography">
        <h3>Photography</h3>
        <p>
            Increase your credibility by getting the most stunning, high-quality
            photos that improve your business image.
        </p>
    </div>
</div>

<style>
    #grids {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: repeat(3, 1fr);
        row-gap: 0;
        column-gap: 0;
    }
    #transform {
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding-right: 100px;
        padding-left: 120px;
        background-color: rgb(255, 251, 247);
    }
    #transform > h3 {
        font-family: "Fraunces", sans-serif;
        font-weight: 900;
        font-size: 32px;
        color: rgb(36, 45, 58);
        margin-bottom: 30px;
    }
    #transform > p {
        font-family: "Barlow", sans-serif;
        color: rgb(112, 110, 123);
        line-height: 1.5;
        margin-bottom: 30px;
    }
    #transform-link > a {
        font-family: "Fraunces", sans-serif;
        text-decoration: none;
        color: rgb(36, 45, 58);
        position: relative;
        z-index: 1;
        letter-spacing: 1px;
    }
    #transform-link > a:hover + #transform-link-bottom {
        background-color: rgb(255, 210, 14);
    }
    #transform-link-bottom {
        width: 140px;
        height: 10px;
        border-radius: 5px;
        background-color: rgb(254, 241, 178);
        position: relative;
        bottom: 10px;
        right: 8px;
        transition: background-color 0.3s;
    }
    #egg > img {
        width: 100%;
        display: block;
    }
    #glass > img {
        width: 100%;
        display: block;
    }
    #standout {
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding-right: 100px;
        padding-left: 120px;
        background-color: rgb(255, 251, 247);
    }
    #standout > h3 {
        font-family: "Fraunces", sans-serif;
        font-weight: 900;
        font-size: 32px;
        color: rgb(36, 45, 58);
        margin-bottom: 30px;
    }
    #standout > p {
        font-family: "Barlow", sans-serif;
        color: rgb(112, 110, 123);
        line-height: 1.5;
        margin-bottom: 30px;
    }
    #standout-link > a {
        font-family: "Fraunces", sans-serif;
        text-decoration: none;
        color: rgb(36, 45, 58);
        position: relative;
        z-index: 1;
        letter-spacing: 1px;
    }
    #standout-link > a:hover + #standout-link-bottom {
        background-color: rgb(255, 108, 91);
    }
    #standout-link-bottom {
        width: 140px;
        height: 10px;
        border-radius: 5px;
        background-color: rgb(255, 216, 207);
        position: relative;
        bottom: 10px;
        right: 8px;
        transition: background-color 0.3s;
    }
    #graphic {
        background-image: url("/assets/desktop/image-graphic-design.jpg");
        background-size: cover;
        display: flex;
        flex-direction: column;
        justify-content: end;
        align-items: center;
        padding: 50px 150px;
    }
    #graphic > h3 {
        font-family: "Fraunces", sans-serif;
        color: rgb(31, 74, 66);
        margin-bottom: 30px;
        font-size: 27px;
    }
    #graphic > p {
        font-family: "Barlow", sans-serif;
        color: rgb(31, 74, 66);
        font-size: 14px;
        text-align: center;
        line-height: 1.5;
    }
    #photography {
        background-image: url("/assets/desktop/image-photography.jpg");
        background-size: cover;
        display: flex;
        flex-direction: column;
        justify-content: end;
        align-items: center;
        padding: 50px 150px;
    }
    #photography > h3 {
        font-family: "Fraunces", sans-serif;
        color: rgb(31, 74, 66);
        margin-bottom: 30px;
        font-size: 27px;
    }
    #photography > p {
        font-family: "Barlow", sans-serif;
        color: rgb(31, 74, 66);
        font-size: 14px;
        text-align: center;
        line-height: 1.5;
    }
</style>
