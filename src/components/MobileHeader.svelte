<script>
    import { openModal } from "../store";
</script>

<div
    class="fixed top-0 left-0 w-screen h-screen border-b bg-white z-50 flex flex-col gap-8 p-5 px-8 md:hidden"
>
    <div class="flex items-center justify-between gap-4 border-b pb-2">
        <h1 class="font-semibold">
            G <span class="text-red-400">YM</span>
        </h1>
        <!-- svelte-ignore a11y_consider_explicit_label -->
        <button
            on:click={() => ($openModal = false)}
            class="outline-none border-none"
        >
            <i class="fa-solid fa-xmark text-2xl"></i>
        </button>
    </div>
    <div class="flex flex-col gap-4 flex-1">
        <button
            on:click={() => reroute("#product")}
            class="border-none outline-none p-2 group duration-200 cursor-pointer text-left"
        >
            <p
                class="duration-200 group-hover:pl-2 poppins text-3xl font-semibold"
            >
                <!-- svelte-ignore element_invalid_self_closing_tag -->
                Product <i class="fa-solid fa-chevron-right text-xl pl-4" />
            </p>
        </button>
        <button
            on:click={() => reroute("#faqs")}
            class="border-none outline-none p-2 group duration-200 cursor-pointer text-left"
        >
            <p
                class="duration-200 group-hover:pl-2 poppins text-3xl font-semibold"
            >
                <!-- svelte-ignore element_invalid_self_closing_tag -->
                FAQs <i class="fa-solid fa-chevron-right text-xl pl-4" />
            </p>
        </button>
        <button
            on:click={() => reroute("#footer")}
            class="border-none outline-none p-2 group duration-200 cursor-pointer text-left"
        >
            <p
                class="duration-200 group-hover:pl-2 poppins text-3xl font-semibold"
            >
                <!-- svelte-ignore element_invalid_self_closing_tag -->
                Contact Info
                <i class="fa-solid fa-chevron-right text-xl pl-4" />
            </p>
        </button>
        <button class="specialBtn">
            <a
                href="mailto:othmane.regragui2020@gmail.com"
                class="duration-200 hover:text-red-400 cursor-pointer"
            >
                <p>Made it By REGRAGUI Othmane</p>
            </a>
        </button>
    </div>
</div>
