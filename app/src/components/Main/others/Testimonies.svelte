<script>
    import Star from '~icons/mdi/star';
    import Title from '../../Texts/Title.svelte';

    const testionies = [
        {
            testimony: "It has been amazing being a frontend developer after enrolling for this course. The support resources, and opportunities provided have helped me refile my skills, work on exciting projects, and grow professionally. iThou is now a part of me.",
            photo: "/testimonies/img1.jpeg",
            name: "Goodluck Nnadi",
            iconTwo: Star
        },
        {
            testimony: "I want to express my heartfelt gratitude for iThou Technology. I'm deeply grateful for the impact on how their technology will continue to shape the future. iThou has been a tech game changer for me and it will for you.",
            photo: "/testimonies/img2.jpeg",
            name: "Jandi Hafsat",
            iconTwo: Star
        },
        {
            testimony: "I am thrilled to be a part of the iThou technology Company team after I enrolled in their program. The collaborative atmosphere, state-of-the-art resources and forward-thinking approach have empowered me to push boundaries, explore new ideas.",
            photo: "/testimonies/img3.jpeg",
            name: "Valeria",
            iconTwo: Star
        }
    ];
</script>

<section class="mt-20 px-5 flex flex-col items-center gap-5">
    <Title text="Testimonies from students" />
    <p>Listen to what our students say about us</p>

    <div class="flex gap-5 flex-col items-center lg:flex-row">
        {#each testionies as { testimony, photo, name, iconTwo }}
            <div class="bg-white shadow-sm shadow-black border rounded-2xl space-y-5 p-7 w-85 testimony-card md:w-90 lg:w-80 xl:w-80 2xl:w-90">
                <p>{testimony}</p>
                <div class="flex gap-5">
                    <div class="overflow-hidden rounded-full w-16 h-16 bg-cover bg-center border-2 border-white" 
                         style={`background-image: url(${photo})`}>
                    </div>
                    <div>
                        <p class="font-semibold">{name}</p>
                        <div class="flex">
                            <svelte:component this={iconTwo} class="text-gold text-sm" />
                            <svelte:component this={iconTwo} class="text-gold text-sm" />
                            <svelte:component this={iconTwo} class="text-gold text-sm" />
                            <svelte:component this={iconTwo} class="text-gold text-sm" />
                            <svelte:component this={iconTwo} class="text-gold text-sm" />
                        </div>
                    </div>
                </div>
            </div>
        {/each}
    </div>
</section>

<style>
    @media (prefers-reduced-motion: no-preference) {
        .testimony-card {
            transform: translateY(70px);
            animation-range: entry 20% cover 50%;
        }

        @keyframes fade-in-up {
            to {
                transform: translateY(0);
            }
        }

        /* Hover effect */
        .testimony-card:hover {
            transform: scale(1.05);
            transition: transform 0.3s ease-in-out;
        }
    }
</style>
