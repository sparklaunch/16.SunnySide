<div id="gallery">
    <img
        src="/assets/desktop/image-gallery-milkbottles.jpg"
        alt="Milk Bottles"
    />
    <img src="/assets/desktop/image-gallery-orange.jpg" alt="Orange" />
    <img src="/assets/desktop/image-gallery-cone.jpg" alt="Cone" />
    <img src="/assets/desktop/image-gallery-sugarcubes.jpg" alt="Sugarcubes" />
</div>

<style>
    #gallery {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
    }
    #gallery > img {
        width: 100%;
        display: block;
    }
</style>
