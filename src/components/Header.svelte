<script>
    import { openModal } from "../store";
</script>

<header class="flex flex-col relative z-20">
    <div
        class="max-w-[1400px] mx-auto w-full flex items-center justify-between p-4 py-6"
    >
        <a href="/">
            <h1 class="font-semibold text-2xl">
                G <span class="text-red-400">YM</span>
            </h1>
        </a>
        <!-- svelte-ignore a11y_consider_explicit_label -->
        <button
            on:click={() => ($openModal = true)}
            class="md:hidden grid place-items-center"
        >
            <i class="fa-solid fa-bars"></i>
        </button>
        <nav class="hidden md:flex items-center gap-4 lg:gap-6">
            <a
                href="#product"
                class="duration-200 hover:text-red-400 cursor-pointer"
                >Product</a
            >
            <a
                href="#faqs"
                class="duration-200 hover:text-red-400 cursor-pointer">FAQs</a
            >
            <a
                href="#footer"
                class="duration-200 hover:text-red-400 cursor-pointer"
                >Contact Info</a
            >
            <button class="specialBtn">
                <a
                    href="mailto:othmane.regragui2020@gmail.com"
                    class="duration-200 hover:text-red-400 cursor-pointer"
                >
                    <p>Made it By REGRAGUI Othmane</p>
                </a>
            </button>
        </nav>
    </div>
</header>
