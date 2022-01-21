<script lang="ts">
    import Social from "$lib/components/Social.svelte";

    const socials = [
        {
            icon: "GitHub-Mark-Light-120px-plus.png",
            alt: "GitHub",
            content: "github.com/zachstence",
            link: "https://www.github.com/zachstence",
        },
        {
            icon: "LI-In-Bug.png",
            alt: "LinkedIn",
            content: "linkedin.com/in/zachary-stence",
            "link": "https://www.linkedin.com/in/zachary-stence",
        },
        {
            icon: "icons8-email-64.png",
            alt: "Email",
            content: "zachstence@gmail.com",
            link: "mailto:zachstence@gmail.com",
        },
    ];
</script>

<section>
    <img src="https://avatars.githubusercontent.com/u/31896377?v=4" alt="Profile" />
    <h1>Zachary Stence</h1>
    <div>
        {#each socials as social}
            <Social {...social} />
        {/each}
    </div>
</section>


<style lang="postcss">
    section {
        @apply flex flex-col items-center justify-center bg-black bg-opacity-50 m-20 p-16 rounded-3xl;
    }

    img {
        @apply w-96 h-96 rounded-full;
    }

    h1 {
        @apply text-5xl mt-8 mb-8;
    }

    div {
        @apply border-2 border-white rounded-md;
    }
</style>