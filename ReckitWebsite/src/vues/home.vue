<template>

    <div>
        <h1 class="mb-4 text-4xl font-extrabold leading-none tracking-tight text-gray-900 md:text-5xl lg:text-6xl dark:text-black">Our Products</h1>
        <p class="mb-6 text-lg font-normal text-gray-500 lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">Here at Reckitt we sell a large varity of medical products to help sooth your illnesses.</p>

        <hr class=" border-black border-8 my-12 w-full">

        <h2 class="mb-4 text-3xl font-extrabold leading-none tracking-tight text-gray-900 md:text-2xl lg:text-4xl dark:text-black">Featured</h2>
        
        <featured></featured>

    </div>

</template>

<script setup>

    import featured  from '../components/featured.vue'

</script>