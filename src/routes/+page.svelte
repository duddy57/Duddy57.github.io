<script>
    AOS.init();

    let habilits = [
        { name: "Golang", Image: "Golang.svg" },
        { name: "Javascript", Image: "Js.svg" },
        { name: "Python", Image: "Python.svg" },
        { name: "React", Image: "React.svg" },
        { name: "Svelte", Image: "Svelte.svg" },
        { name: "Tailwind", Image: "Tailwind.svg" },
        { name: "Linux", Image: "Linux.svg" },
    ];

    let benefits = [
        {
            name: "Entusiasta do Desenvolvimento FrontEnd",
            label: "Sou um apaixonado desenvolvedor FrontEnd em constante busca por desafios e crescimento. Minhas habilidades destacam-se em tecnologias como GoLang, SvelteKit e Tailwind, onde a elegância e a eficiência se encontram em cada linha de código.",
        },
        {
            name: " Transformando Ideias em Realidade",
            label: "Dedicado e proativo, minha paixão é transformar ideias em interfaces visuais impactantes. Acredito na harmonia entre design e desenvolvimento para criar produtos memoráveis.",
        },
        {
            name: "Explorando o Mundo do FrontEnd",
            label: "Estou animado para explorar mais no vasto mundo do FrontEnd, superar desafios e colaborar em projetos inovadores. Seja bem-vindo à minha jornada, onde a criatividade é a essência de cada código.",
        },
        {
            name: "Construindo um Futuro Digital Inspirador",
            label: "Juntos, podemos construir um futuro digital inspirador! Estou aqui para superar desafios, explorar novas possibilidades e colaborar em projetos que fazem a diferença.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10 z-[10] mt-8"
        >
            <h2
                class="font-semibold text-4xl sm:text-5xl md:text-6xl bg-clip-text text-transparent bg-gradient-to-r from-[#b57bee] to-[#8364e8]"
            >
                Ola! me chamo Alexsandro <br />
                Front-End Developer
            </h2>
            <p class="text-lg sm:text-lg md:text-xl">
                Bem-vindo ao meu mundo digital! Sou Alexsandro, apaixonado por
                transformar ideias em
                <span
                    class="bg-clip-text text-transparent bg-gradient-to-r from-[#b57bee] to-[#8364e8] poppins"
                    >experiências envolventes</span
                >. Navegue pelos meus projetos e descubra como a magia do
                FrontEnd ganha vida
            </p>
        </div>
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10 z-[10] mt-8 font."
        >
            <a
                href="#projects"
                class="mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full backdrop-blur-md bg-transparent text-white border border-violet-400
                 cursor-pointer"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-gradient-to-r from-[#905dc2] to-[#8364e8] group-hover:translate-x-full z-0 duration-200"
                ></div>
                <h4 class="relative z-9">
                    Inicie sua Jornada <br />pelo meu mundo
                </h4>
            </a>
            <div class="flex flex-row justify-center gap-14 mt-10">
                <a
                    href="https://www.linkedin.com/in/duddy57dev"
                    target="_blank"
                    class="transition ease-in-out hover:-translate-y-3 hover:scale-110"
                    ><i
                        class=" fa-brands fa-linkedin fa-2xl text-violet-400 hover:text-violet-600"
                    ></i></a
                >
                <a
                    href="https://github.com/duddy57"
                    target="_blank"
                    class="transition ease-in-out hover:-translate-y-3 hover:scale-110"
                    ><i
                        class="fa-brands fa-github fa-2xl text-violet-400 hover:text-violet-600"
                    ></i></a
                >
                <a
                    href="https://www.instagram.com/duddy57dev_"
                    class="transition ease-in-out hover:-translate-y-3 hover:scale-110"
                    target="_blank"
                    ><i
                        class="fa-brands fa-instagram fa-2xl text-violet-400 hover:text-violet-600"
                    ></i></a
                >
            </div>
        </div>
    </section>
    <section
        id="about"
        class=" py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative z-30 backdrop-blur-sm bg-transparent"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0
             before:left-0 before:w-2/3 before:h-1.5 before:bg-gradient-to-r from-[#b57bee] to-[#8364e8] after:absolute after:bottom-0
             after:right-0 after:w-2/3 after:h-1.5 after:bg-gradient-to-l py-4"
        >
            <h6 class="text-lg sm:text-xl md:text-3xl z-10">
                Um pouco <span
                    class="bg-gradient-to-r from-[#b57bee] to-[#8364e8] poppins bg-clip-text text-transparent"
                    >sobre mim</span
                >
            </h6>
        </div>

        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            Eu sou. . .
        </p>
        {#each benefits as benefit, index}
            <div class="flex flex-wrap">
                <p
                    class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                >
                    0{index + 1}
                </p>
                <div class="w-full md:w-full p-4" data-aos="fade-up">
                    <h2 class="text-3xl font-bold mb-4 text-violet-400">
                        {benefit.name}
                    </h2>
                    <p class="text-lg">
                        {benefit.label}
                    </p>
                </div>
            </div>
        {/each}
    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0
         before:left-0 before:w-2/3 before:h-1.5 before:bg-gradient-to-r from-[#b57bee] to-[#8364e8] after:absolute after:bottom-0
         after:right-0 after:w-2/3 after:h-1.5 after:bg-gradient-to-l py-4"
        >
            <h6 class="text-lg sm:text-xl md:text-3xl z-10">
                Alguns dos <span
                    class="bg-gradient-to-r from-[#b57bee] to-[#8364e8] poppins bg-clip-text text-transparent"
                >
                    meus
                </span> projetos
            </h6>
        </div>
    </section>
    <section id="skils">
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0
         before:left-0 before:w-2/3 before:h-1.5 before:bg-gradient-to-r from-[#b57bee] to-[#8364e8] after:absolute after:bottom-0
         after:right-0 after:w-2/3 after:h-1.5 after:bg-gradient-to-l py-4"
        >
            <h6 class="text-lg sm:text-xl md:text-3xl z-10">
                <span
                    class="bg-gradient-to-r from-[#b57bee] to-[#8364e8] poppins bg-clip-text text-transparent"
                >
                    Minhas</span
                > habilidades em tecnologia incluem
            </h6>
        </div>
        <div class="flex flex-row sm:flex-col  items-center sm:mt-20 mt-10">
            <div
                class="flex flex-wrap justify-center text-center gap-40 flex-row"
            >
                <div class="flex flex-col">
                    <div class="group relative">
                        <div
                            class="lg:w-24 lg:h-24 w-16 h-16 mx-4 my-4 shadow-lg rounded-lg overflow-hidden hover:shadow-xl transition duration-300 ease-in-out"
                        >
                            <img src="JS.svg" class=" z-20" alt="Js-Icon" />
                        </div>
                        <div
                            class="absolute inset-0 bg-yellow-400 opacity-0 group-hover:rounded-lg group-hover:opacity-50 duration-300 ease-in-out group-hover:blur-sm"
                        ></div>
                    </div>
                    <h6
                        class=" poppins text-center text-[#FFE66D] rounded-xl bg-slate-900"
                    >
                        Javascript
                    </h6>
                </div>

                <div class="flex flex-col">
                    <div class="group relative">
                        <div
                            class=" lg:w-24 lg:h-24 w-16 h-16 mx-4 my-4 shadow-lg rounded-lg overflow-hidden hover:shadow-xl transition duration-300 ease-in-out"
                        >
                            <img src="Golang.svg" class=" z-20" alt="Js-Icon" />
                        </div>
                        <div
                            class="absolute inset-0 bg-[#73CFDE] opacity-0 group-hover:rounded-lg group-hover:opacity-50 duration-300 ease-in-out group-hover:blur-sm"
                        ></div>
                    </div>
                    <h6
                        class=" poppins text-center text-[#73CFDE] rounded-xl bg-slate-900"
                    >
                        Golang
                    </h6>
                </div>

                <div class="flex flex-col">
                    <div class="group relative">
                        <div
                            class="lg:w-24 lg:h-24 w-16 h-16 mx-4 my-4 shadow-lg rounded-lg overflow-hidden hover:shadow-xl transition duration-300 ease-in-out"
                        >
                            <img
                                src="Tailwind.svg"
                                class=" z-20"
                                alt="Js-Icon"
                            />
                        </div>
                        <div
                            class="absolute inset-0 bg-[#18BAB9] opacity-0 group-hover:rounded-lg group-hover:opacity-50 duration-300 ease-in-out group-hover:blur-sm"
                        ></div>
                    </div>
                    <h6
                        class=" poppins text-center text-[#18BAB9] rounded-xl bg-slate-900"
                    >
                        Tailwind
                    </h6>
                </div>
            </div>

            <div
                class="flex flex-wrap justify-center text-center gap-40 flex-row mt-28"
            >
                <div class="flex flex-col">
                    <div class="group relative">
                        <div
                            class="lg:w-24 lg:h-24 w-16 h-16 mx-4 my-4 shadow-lg rounded-lg overflow-hidden hover:shadow-xl transition duration-300 ease-in-out"
                        >
                            <img
                                src="React.svg"
                                class=" z-20"
                                alt="React-Icon"
                            />
                        </div>
                        <div
                            class="absolute inset-0 bg-[#05D7FB] opacity-0 group-hover:rounded-lg group-hover:opacity-50 duration-300 ease-in-out group-hover:blur-sm"
                        ></div>
                    </div>
                    <h6
                        class=" poppins text-center text-[#05D7FB] rounded-xl bg-slate-900"
                    >
                        React
                    </h6>
                </div>

                <div class="flex flex-col">
                    <div class="group relative">
                        <div
                            class="lg:w-24 lg:h-24 w-16 h-16 mx-4 my-4 shadow-lg rounded-lg overflow-hidden hover:shadow-xl transition duration-300 ease-in-out"
                        >
                            <img
                                src="Svelte.svg"
                                class="w-20 h-20 z-20 text-right"
                                alt="Svelte-Icon"
                            />
                        </div>
                        <div
                            class="absolute inset-0 bg-[#a27824] opacity-0 group-hover:rounded-lg group-hover:opacity-50 duration-300 ease-in-out group-hover:blur-sm"
                        ></div>
                    </div>
                    <h6
                        class=" poppins text-center text-[#a27824] rounded-xl bg-slate-900"
                    >
                        Svelte
                    </h6>
                </div>

                <div class="flex flex-col">
                    <div class="group relative">
                        <div
                            class="lg:w-24 lg:h-24 w-16 h-16 mx-4 my-4 shadow-lg rounded-lg overflow-hidden hover:shadow-xl transition duration-300 ease-in-out"
                        >
                            <img
                                src="Linux.svg"
                                class="z-20"
                                alt="Linux-Icon"
                            />
                        </div>
                        <div
                            class="absolute inset-0 bg-gray-600 opacity-0 group-hover:rounded-lg group-hover:opacity-50 duration-300 ease-in-out group-hover:blur-sm"
                        ></div>
                    </div>
                    <h6
                        class=" poppins text-center text-white rounded-xl bg-slate-900"
                    >
                        Linux
                    </h6>
                </div>
            </div>
        </div>

        <h5
            class="text-center mx-auto text-2xl sm:text-3xl font-semibold poppins mt-20"
        >
            Após isso <span
                class="bg-gradient-to-r from-[#b57bee] to-[#8364e8] poppins bg-clip-text text-transparent"
                >porque</span
            >
            não da uma
            <span
                class="bg-gradient-to-r from-[#b57bee] to-[#8364e8] poppins bg-clip-text text-transparent"
            >
                chance?</span
            >
        </h5>
    </section>
</main>
