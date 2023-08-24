<svelte:head>
    <title>Главная страница</title>
</svelte:head>

<div class="container">
    <div class="info">
        <div class="animate-background">
            <div class="container info-container">
                <div class="info-text">
                    <h1> 
                        <p class="animate-text-1">Любимый сериал|телефильм.</p>
                        <p class="text-2">"17 мгновений весны". </p>
                    </h1>
                </div>
                <h2 class="subtitle">Сегодня мне бы хотелось рассказать о своем самом любимом телефильме. А именно о "17 мгновениях весны", читайте далее и узнаете полную рецензию в рамках 5й аттестационной работы!</h2>
                <!-- svelte-ignore a11y-no-noninteractive-tabindex -->
                <div style="color: black;" class="scroll-button animate-scroll" tabindex="0">
                    <a href="/about" class="about-link"><span>Читайте далее!</span></a>
                </div>
            </div>
        </div>
    </div>
</div>
<div class="background-div"></div>

<style>
    .info {
        text-align: center;
        position: relative;
    }
    .info-container {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        text-align: left;
        align-items: start;
    }
    .container {
        max-width: 1400px;
        margin: 190px 0 0 2.5rem;
    }
    .info h1 {
        font-size: 4rem;
        margin: 0;
    }
    .info h1 p {
        position: relative;
        font: inherit;
        margin: 0;
        text-align: left;
        line-height: 130%;
        width: fit-content;
        font-weight: 800;
        letter-spacing: -0.03em;
    }
    .info h2 {
        max-width: 65ch;
        font-weight: 200;
        margin-top: 0.50rem;
    }
    .background-div {
        background-color: #ecebe8;
        width: 100%;
        height: 56vh;
        margin: -205px auto;
    }
    .info .info-text {
        position: relative;  
    }
    .scroll-button {
        display: flex;
        border: none;
        outline: none;
        cursor: pointer;
    }
    .about-link {
        text-decoration: none;
        display: inline-block;
        margin: 10px;
        color: rgb(0, 0, 0);
        box-shadow: 0 0 0 2px white;
        padding: 20px 0;
        width: 150px;
        text-align: center;
        text-transform: uppercase;
        letter-spacing: 3px;
        position: relative;
        overflow: hidden;
    }
    .about-link span {
        font-family: 'Montserrat', sans-serif;
        position: relative;
        z-index: 5;
    }
    .about-link::before, .about-link:after {
        content: "";
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        left: 0;
    }
    .about-link:before {
        transform: translateX(-100%);
        background: rgb(118, 117, 117);
        transition: transform .3s cubic-bezier(.55, .055, .675, .19);
    }
    .about-link:after {
        background: #ffffff;
        transform: translateX(100%);
        transition: transform .3s cubic-bezier(.16, .73, .58, .62) .3s;
    }
    .about-link:hover:before, .about-link:hover:after {
        transform: translateX(0);
    }
</style>