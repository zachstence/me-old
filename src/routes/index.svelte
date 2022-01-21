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

<main>
    <section>
        <img src="https://avatars.githubusercontent.com/u/31896377?v=4" alt="Profile" />
        <h1>Zachary Stence</h1>
        <div>
            {#each socials as social}
                <Social {...social} />
            {/each}
        </div>
    </section>
</main>


<style lang="postcss">
    main {
        @apply h-screen w-screen flex items-center justify-center bg-black;
        background-color: #090909;
        background-image: url("data:image/svg+xml,%3Csvg width='6' height='6' viewBox='0 0 6 6' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='%23e9f6ff' fill-opacity='0.075' fill-rule='evenodd'%3E%3Cpath d='M5 0h1L0 6V5zM6 5v1H5z'/%3E%3C/g%3E%3C/svg%3E");
    }

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