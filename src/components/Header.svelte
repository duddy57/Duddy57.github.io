<script>
    export let y;

    let tabs = [
        { name: "#about", label: "Sobre mim" },
        { name: "#projects", label: "Projetos" },
        { name: "#skils", label: "Habilidades" },
    ];
</script>

<header
    class={"sticky z-50 top-0 duration-200 px-8 flex items-center justify-between border border-solid backdrop-blur-sm bg-transparent" +
        (y > 0
            ? " py-4 bg-slate-950 border-violet-950"
            : " py-6 bg-transparent border-transparent")}
>
    <a href="/"><img src="Logo.svg" alt="Logo" class=" h-10 w-10" /></a>
    <div class="sm:flex items-center gap-6 hidden font-bold">
        {#each tabs as tab, index}
            <a href={tab.name} class=" duration-200 hover:text-violet-400">
                <p>{tab.label}</p>
            </a>
        {/each}
        <a
            href="#Footer"
            class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950"
        >
            <div
                class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
            ></div>
            <h4 class="relative z-9">Contato</h4>
        </a>
    </div>
</header>
