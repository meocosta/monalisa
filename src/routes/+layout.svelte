<script>
    import "./page.scss";
    let username = "Maria Elisa";
    let cor = "#218380";
</script>

<section id="intro">
    <h2>bem vindo ao meu website!</h2>

    <nav>
        <a href="/sobre">sobre mim</a>
        <a href="/projetos">projetos</a>
    </nav>

    <hr id="dourado" />
    <h1>
        <!-- svelte-ignore a11y_no_static_element_interactions -->
        Portifólio da <span
            onmouseenter={() => {
                username = "Monalisa";
                cor = "#FFBC42";
            }}
            onmouseleave={() => {
                username = "Maria Elisa";
                cor = "#218380";
            }}
            style="color: {cor}">{username}</span
        >
    </h1>
    <hr id="dourado" />
</section>

<slot></slot>