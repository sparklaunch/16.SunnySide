<script lang="ts">
    interface Testimonial {
        name: string;
        title: string;
        content: string;
        profile: string;
    }
    const testimonials: Testimonial[] = [
        {
            name: "Emily R.",
            title: "Marketing Director",
            content:
                "We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.",
            profile: "image-emily.jpg"
        },
        {
            name: "Thomas S.",
            title: "Chief Operating Officer",
            content:
                "Sunnyside's enthusiasm coupled with their keen interest in our brand's success made it a satisfying and enjoyable experience.",
            profile: "image-thomas.jpg"
        },
        {
            name: "Jennie F.",
            title: "Business Owner",
            content:
                "Incredible end result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!",
            profile: "image-jennie.jpg"
        }
    ];
</script>

<div id="testimonials">
    <h3>CLIENT TESTIMONIALS</h3>
    <div id="items">
        {#each testimonials as testimonial}
            <div class="testimonial">
                <img
                    class="profile"
                    src="/assets/{testimonial.profile}"
                    alt={testimonial.name}
                />
                <p class="content">{testimonial.content}</p>
                <h4 class="name">{testimonial.name}</h4>
                <p class="title">{testimonial.title}</p>
            </div>
        {/each}
    </div>
</div>

<style>
    #testimonials {
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: rgb(255, 251, 247);
        padding: 150px 0;
    }
    #testimonials > h3 {
        font-family: "Fraunces", sans-serif;
        color: rgb(153, 154, 157);
        letter-spacing: 3px;
        margin-bottom: 50px;
    }
    #items {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        column-gap: 30px;
    }
    .testimonial {
        width: 300px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .testimonial > .profile {
        width: 50px;
        height: 50px;
        border-radius: 50%;
        margin-bottom: 50px;
    }
    .testimonial > .content {
        font-family: "Barlow";
        color: rgb(87, 89, 94);
        line-height: 1.5;
        text-align: center;
        margin-bottom: 50px;
    }
    .testimonial > .name {
        font-family: "Fraunces", sans-serif;
        color: rgb(24, 40, 52);
        margin-bottom: 10px;
    }
    .testimonial > .title {
        font-family: "Barlow", sans-serif;
        color: rgb(180, 180, 180);
        font-size: 14px;
    }
</style>
