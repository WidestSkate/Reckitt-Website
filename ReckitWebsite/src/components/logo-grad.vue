<template>
	<div class="gradient-background overflow-hidden h-custom " >
		<div class="grid grid-cols-1 md:grid-cols-2 text-center">
			<div class="pt-20">
				<h1 class="mb-4 text-4xl font-extrabold leading-none pt-32 tracking-tight md:text-5xl lg:text-6xl text-white">Reckitt Products</h1>
				<p class="mb-6 text-lg font-normal lg:text-xl sm:px-16 xl:px-48 text-white">Reckitt has many products designed to help sooth your illnesses</p>
			</div>
			<svg class="hidden md:block" viewBox="0 0 950 700">
				<path opacity="1" d="M435.425 -60C196.108 -60 1.0047 126.583 1.0047 388.995C0.564981 471.386 19.1446 552.767 55.2973 626.804L164.492 550.352C139.468 496.086 126.809 436.939 127.43 377.184C127.43 190.22 264.633 48.6072 440.563 48.6072C612.42 48.6072 717.94 169.795 717.94 326.247C717.94 466.209 624.757 557.113 503.886 557.113C388.264 557.113 306.608 477.928 306.608 365.262C306.608 265.966 369.426 199.486 445.07 199.486C501.914 199.486 533.041 226.254 533.041 266.868C533.041 313.422 484.9 339.394 435.561 325.576L383.148 362.275C417.195 411.004 498.754 481.54 532.955 503.219C533.131 503.102 588.144 464.573 588.144 464.573C556.963 440.918 527.237 415.403 499.129 388.167C574.965 375.63 609.236 320.477 609.236 266.554C609.236 182.896 549.654 123.797 445.832 123.797C322.329 123.797 218.951 225.348 218.951 370.147C218.951 530.757 336.411 649.72 505.356 649.72C691.941 649.72 824 510.471 824 323.023C824 101.875 670.532 -60 435.425 -60Z" fill="white"></path>
			</svg>
		</div>
	</div>
</template>

<script setup>
	
</script>

<style scoped>

.h-custom {
	height: 35rem;
}

.gradient-background {
  background: linear-gradient(90deg,#ff1c6a,#ff4d46);
  background-size: 120% 120%;
  animation: gradient-animation 20s ease infinite;
}

@keyframes gradient-animation {
  0% {
    background-position: 0% 50%;
  }
  75% {
    background-position: 100% 50%;
  }
  120% {
    background-position: 0% 50%;
  }
}
</style>
