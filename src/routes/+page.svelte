<script>
    import Works from "../components/works-page.svelte";
    import heroimg from "$lib/assets/hero-img.jpg";
</script>

<div class="hero-wrapper">
    <h1 class="name">Yashu Maurya</h1>
    <div class="description-box">
        <p class="description">
            Engineering Student • Embedded Systems • Machine Learning • Mathematics
        </p>
    </div>
    <a href="mailto:yashuff1@gmail.com" class="email">yashuff1@gmail.com</a>
    <div class="link-wrapper">
        <a href="https://github.com/Yashu-Maurya" class="link">Github</a>
        <img src={heroimg} alt="" class="hero-image">
        <a href="https://linkedin.com/" class="link">Linkedin</a>
    </div>
</div>
<div class="separator"></div>
<Works></Works>

<style>

    .hero-wrapper {
        display: flex;
        flex-direction: column;
        max-width: 1234px;
        padding: 16px;
        margin: auto auto;

        font-family: 'inter';

    }

    .hero-image {
        width: 100px;
    }

    .name {
        font-size: 96px;   
        font-weight: bold;   
        margin: 16px 0px;
    }
    .email {
        font-size: 16px;
        text-decoration: none; 
        text-align: end;
    }

    .description-box {
        align-self: flex-end;
        max-width: 320px;
        padding: 8px;

        text-align: end;
        text-justify: auto;

        border-style: solid;
        border-color: transparent transparent transparent black;
        border-width: 2px;
        border-radius: 0px 0px 0px 16px;


    }

    .link-wrapper {
        display: flex;
        width: 100%;
        justify-content:space-between;
        align-items:baseline;
        align-self: flex-start;

        padding-top: 46px;
        text-align: start;
        text-justify: auto;

    }

    .link {
        text-decoration: none;
        font-size: 18px;
        color: blue;
        font-family: monospace;
    }

    .separator {
        border-style: solid;
        border-width: 5px;
        border-color: black;
        margin-top: 48px;
    }
</style>