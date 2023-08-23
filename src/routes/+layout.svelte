<nav>
    <div class="nav-container">
        <a href="/" сlass="main-link" title="Вернуться на главную">Мой любимый сериал</a>
        <div class="nav-links">
            {#each nav as link}
            {#if link.isShow}
                <a href={link.href} class="link">{link.title}</a>
                {/if}
            {/each}
        </div>
    </div>
</nav>

<div class="container">
    <!--Pages will be injected below-->
    <slot></slot>
</div>
<script>
    const nav= [
        {
            title:'Фильм',
            href: '/about',
            isShow: true
        },
        {
            title:'Любимые персонажи',
            href: '/blog',
            isShow: true
        },
        {
            title:'Портфолио',
            href: '/project',
            isShow: true
        },
        {
            title:'Контакты',
            href: '/contact',
            isShow: true
        },
        {
            title:'temp',
            href: '/temp',
            isShow: false
        }       
    ]
</script>
<style>
    .container {
        max-width: 1400px;
        margin: 50px auto;
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