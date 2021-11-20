<script lang="ts">
    export let icon: string;
    export let alt: string;
    export let content: string;
    export let link: string;
</script>

<a href={link}>
    <img src={icon} {alt} />
    <span>{content}</span>
</a>


<style lang="postcss">
    a {
        @apply flex items-center 
            m-2 p-2
            box-border w-auto
            border-2 border-transparent rounded-md;
        width: fit-content;
    }

    a:hover {
        @apply border-white;
    }


    img {
        @apply w-8 h-8 mr-4;
    }
</style>