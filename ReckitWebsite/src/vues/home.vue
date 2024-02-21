<template>

    <div>

	<gradient></gradient>

        <hr class=" border-black border-8 my-12 w-full">

        <h2 class="mb-8 text-3xl font-extrabold leading-none tracking-tight text-gray-900 md:text-2xl  lg:text-4xl dark:text-black">Featured</h2>
        
        <featured></featured>

    </div>

</template>

<script setup>

	import featured  from '../components/featured.vue'
	import gradient from '../components/logo-grad.vue'
</script>
