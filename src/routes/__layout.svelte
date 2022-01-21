<script>
  import "../app.css";
</script>


<main>
    <slot />
</main>


<style lang="postcss">
    main {
        @apply h-screen w-screen flex items-center justify-center bg-black;
        background-color: #090909;
        background-image: url("data:image/svg+xml,%3Csvg width='6' height='6' viewBox='0 0 6 6' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='%23e9f6ff' fill-opacity='0.075' fill-rule='evenodd'%3E%3Cpath d='M5 0h1L0 6V5zM6 5v1H5z'/%3E%3C/g%3E%3C/svg%3E");
    }
</style>