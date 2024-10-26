<script>
    import Section from "./Section.svelte";
    let faqs = [
        {
            question: "What is Swoley Moley?",
            ans: "Swoley Moley is a fun fitness app designed to make your workouts enjoyable by incorporating interactive games and challenges.",
        },
        {
            question: "How do I download Swoley Moley?",
            ans: "You can download Swoley Moley from the App Store (for iOS) or Google Play Store (for Android) on your mobile device.",
        },
        {
            question: "Is Swoley Moley free to use?",
            ans: "Yes, Swoley Moley offers a free version with basic features. There is also a premium subscription that unlocks additional games and advanced workout tracking.",
        },
        {
            question: "What types of workouts does Swoley Moley offer?",
            ans: "Swoley Moley offers a variety of workouts, including cardio, strength training, and flexibility exercises. The workouts are designed to be engaging and entertaining.",
        },
        {
            question: "Can I connect Swoley Moley to my fitness tracker?",
            ans: "Yes, Swoley Moley supports integration with popular fitness trackers, allowing you to sync your workout data and track your progress seamlessly.",
        },
    ];
</script>

<Section id="faqs">
    <div
        class="flex flex-col gap-10 sm:gap-14 md:gap-24 py-20 flex-1 items-center justify-center"
    >
        <div class="flex flex-col gap-2">
            <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
                For all your questions, qualms & queries
            </p>
            <h3
                class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
            >
                Frequently Asked Questions
            </h3>
        </div>
        <div class="flex flex-col gap-8 sm:gap-10 md:gap-14 w-full">
            {#each faqs as faq}
                <div
                    class="flex flex-col gap-2 text-left max-w-[800px] w-full mx-auto relative p-4 px-6"
                >
                    <div
                        class="absolute top-0 left-0 w-1/3 h-[1px] bg-slate-950 -translate-x-4"
                    ></div>
                    <div
                        class="absolute top-0 left-0 h-2/3 w-[1px] bg-slate-950 -translate-y-4"
                    ></div>
                    <h4 class="text-lg sm:text-xl md:text-2xl pt-2">
                        {faq.question}
                    </h4>
                    <p class="pl-2">{faq.ans}</p>
                </div>
            {/each}
        </div>
    </div>
</Section>
