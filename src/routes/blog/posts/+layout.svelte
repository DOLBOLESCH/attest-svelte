<div class="container">
    <a href="/blog" class="link"><strong>В начало!</strong></a>
    <slot />
</div>
<style>
    .container {
        margin: 50px auto;
        max-width: 800px;
        padding: 0 20px;
    }

    .link {
        text-decoration: none;
        display: inline-block;
        padding: 10px 30px;
        margin: 10px 20px;
        position: relative;
        overflow: hidden;
        border: 2px solid #000000;
        border-radius: 8px;
        font-family: 'Montserrat', sans-serif;
        color: #000000;
        transition: .2s ease-in-out;
    }
    .link:before {
        content: "";
        background: linear-gradient(90deg, rgba(255, 255, 255, .1), rgba(255, 255, 255, .5));
        height: 50px;
        width: 50px;
        position: absolute;
        top: -8px;
        left: -75px;
        transform: skewX(-45deg);
    }
    .link:hover {
        background: #000000;
        color: #fff;
    }
    .link:hover:before {
        left: 150px;
        transition: .5s ease-in-out;
    } 
</style> 