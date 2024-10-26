<script>
    import Section from "./Section.svelte";
    import Header from "./Header.svelte";
    export let dark;
</script>

<Section>
    <Header />
    <div
        class="flex flex-col gap-10 flex-1 items-center justify-center pb-10 md:pb-14"
    >
        <h2
            class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl max-w-[1000px] mx-auto w-full text-center font-bold tracking-tight leading-snug"
        >
            <span class="text-red-500">Gym</span> Training
            <span class="text-gray-500 line-through">Can Be Tough</span><br />
            Just Got <span class="text-red-500">Simpler</span>
        </h2>

        <p
            class="text-2xl sm:text-3xl md:text-4xl text-left max-w-[900px] mx-auto w-full font-semibold tracking-wide leading-relaxed"
        >
            Take action with confidence! Your personal trainer is now in your
            pocket, offering <span class="italic"
                >custom workouts, clear exercise guidance, in-depth progress
                tracking</span
            > and so much more.
        </p>

        <div class="flex items-center gap-4">
            <button class={"specialBtn " + (dark ? " bg-[#181b34]" : " ")}>
                <p class="text-base sm:text-lg md:text-xl">Contact Us</p>
            </button>
        </div>
    </div>
</Section>
