<script>
    import ProductCard from "./ProductCard.svelte";
    import Section from "./Section.svelte";
    let productFeatures = [
        {
            featureList: [
                "Track daily progress",
                "Detailed weights and reps logging",
                "Engage in community challenges",
                "Fresh workouts each day",
            ],
            description:
                "Swoley moley provides all the tools and guidance needed to train with confidence and effectiveness.",
            imgUrl: "https://images.pexels.com/photos/1229356/pexels-photo-1229356.jpeg?auto=compress&cs=tinysrgb&w=600",
        },
        {
            featureList: [
                "Set personal preferences",
                "Tailored workout plans",
                "Adaptable training routines",
                "Progress across key exercises",
            ],
            description:
                "Build consistency and visualize your journey with our comprehensive tracking and analytics features.",
            imgUrl: "https://images.pexels.com/photos/1954524/pexels-photo-1954524.jpeg?auto=compress&cs=tinysrgb&w=600",
        },
        {
            featureList: [
                "Remove training guesswork",
                "Efficient time use",
                "Reach peak performance",
                "Develop functional strength",
            ],
            description:
                "Provide as much personal information as desired to ensure every workout aligns with your goals.",
            imgUrl: "https://images.pexels.com/photos/414029/pexels-photo-414029.jpeg?auto=compress&cs=tinysrgb&w=600",
        },
        {
            featureList: [
                "User-friendly interface",
                "Progressive workout challenges",
                "Holistic wellness tracking",
                "Expert-guided routines",
            ],
            description:
                "Navigate your fitness journey seamlessly with features designed to support holistic growth and well-being.",
            imgUrl: "https://images.pexels.com/photos/136404/pexels-photo-136404.jpeg?auto=compress&cs=tinysrgb&w=600",
        },
    ];
</script>

<Section id="product">
    <div
        class="flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center pb-10 md:pb-14"
    >
        <div class="flex flex-col gap-2">
            <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
                Start your lifetime <span class="text-red-400">gym streak</span>
                today
            </p>
            <h3
                class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
            >
                Features For Everyone
            </h3>
        </div>

        {#each productFeatures as productFeature, index}
            <ProductCard {productFeature} {index}>
                {#if index === 0}
                    Experience a beginner exercise <span
                        class="text-red-400 font-medium">master</span
                    > class
                {:else if index === 1}
                    Lay the foundations for <span
                        class="text-red-400 font-medium">routine</span
                    > and consistency
                {:else}
                    Workouts specific to your <span
                        class="text-red-400 font-medium">environment</span
                    >
                    and
                    <span class="text-red-400 font-medium">expertise</span>
                {/if}
            </ProductCard>
        {/each}
    </div>
</Section>
