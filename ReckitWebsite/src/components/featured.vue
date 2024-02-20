<template>
    <div id="carousel-example" class="relative w-full" data-carousel="slide">
    <!-- Carousel wrapper -->
    <div class="relative h-56 overflow-hidden rounded-lg sm:h-64 xl:h-80 2xl:h-96">
        <!-- Item 1 -->
        <div id="carousel-item-1" class="hidden duration-700 ease-in-out">
            <img
                src="https://www.gaviscon.co.uk/static/486a5e83388af61137ee70177892c754/35871/nggz7grjrjf7jfdibkbo.webp"
                class="absolute left-1/2 top-1/2 block w-full -translate-x-1/2 -translate-y-1/2"
                alt="..."
            />
            <h1>HELLO!</h1>
        </div>
        <!-- Item 2 -->
        <div id="carousel-item-2" class="hidden duration-700 ease-in-out">
            <img
                src="https://www.gaviscon.co.uk/static/486a5e83388af61137ee70177892c754/35871/nggz7grjrjf7jfdibkbo.webp"
                class="absolute left-1/2 top-1/2 block w-full -translate-x-1/2 -translate-y-1/2"
                alt="..."
            />
            <h1>ndfgndfvvd!</h1>

        </div>
        <!-- Item 3 -->
        <div id="carousel-item-3" class="hidden duration-700 ease-in-out">
            <img
                src="https://www.gaviscon.co.uk/static/486a5e83388af61137ee70177892c754/35871/nggz7grjrjf7jfdibkbo.webp"
                class="absolute left-1/2 top-1/2 block w-full -translate-x-1/2 -translate-y-1/2"
                alt="..."
            />
            <h1>HELrgsdcvsgnLO!</h1>

        </div>
        <!-- Item 4 -->
        <div id="carousel-item-4" class="hidden duration-700 ease-in-out">
            <h1>gsrgr!</h1>
            <img
                src="https://www.gaviscon.co.uk/static/486a5e83388af61137ee70177892c754/35871/nggz7grjrjf7jfdibkbo.webp"
                class="absolute left-1/2 top-1/2 block w-full -translate-x-1/2 -translate-y-1/2"
                alt="..."
            />
        </div>
    </div>
    <!-- Slider indicators -->
    <div
        class="absolute -bottom-9 left-1/2 z-30 flex -translate-x-1/2 space-x-3 rtl:space-x-reverse"
    >
        <button
            id="carousel-indicator-1"
            type="button"
            class="h-3 w-3 rounded-full"
            aria-current="true"
            aria-label="Slide 1"
        ></button>
        <button
            id="carousel-indicator-2"
            type="button"
            class="h-3 w-3 rounded-full"
            aria-current="false"
            aria-label="Slide 2"
        ></button>
        <button
            id="carousel-indicator-3"
            type="button"
            class="h-3 w-3 rounded-full"
            aria-current="false"
            aria-label="Slide 3"
        ></button>
        <button
            id="carousel-indicator-4"
            type="button"
            class="h-3 w-3 rounded-full"
            aria-current="false"
            aria-label="Slide 4"
        ></button>
    </div>
    <!-- Slider controls -->
    <button
        id="data-carousel-prev"
        type="button"
        class="group absolute left-0 top-0 z-30 flex h-full cursor-pointer items-center justify-center px-4 focus:outline-none"
    >
        <span
            class="inline-flex h-10 w-10 items-center justify-center rounded-full bg-white/30 group-hover:bg-white/50 group-focus:outline-none group-focus:ring-4 group-focus:ring-white dark:bg-gray-800/30 dark:group-hover:bg-gray-800/60 dark:group-focus:ring-gray-800/70"
        >
            <svg
                class="h-4 w-4 text-white dark:text-gray-800"
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 6 10"
            >
                <path
                    stroke="currentColor"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M5 1 1 5l4 4"
                />
            </svg>
            <span class="hidden">Previous</span>
        </span>
    </button>
    <button
        id="data-carousel-next"
        type="button"
        class="group absolute right-0 top-0 z-30 flex h-full cursor-pointer items-center justify-center px-4 focus:outline-none"
    >
        <span
            class="inline-flex h-10 w-10 items-center justify-center rounded-full bg-white/30 group-hover:bg-white/50 group-focus:outline-none group-focus:ring-4 group-focus:ring-white dark:bg-gray-800/30 dark:group-hover:bg-gray-800/60 dark:group-focus:ring-gray-800/70"
        >
            <svg
                class="h-4 w-4 text-white dark:text-gray-800"
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 6 10"
            >
                <path
                    stroke="currentColor"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="m1 9 4-4-4-4"
                />
            </svg>
            <span class="hidden">Next</span>
        </span>
    </button>
</div>
</template>
  
  <script setup>
  import { onMounted } from 'vue';
  import { initFlowbite, Carousel } from 'flowbite'


  onMounted(() => {

    initFlowbite();

    const carouselElement = document.getElementById('carousel-example');

    const items = [
        {
            position: 0,
            el: document.getElementById('carousel-item-1'),
        },
        {
            position: 1,
            el: document.getElementById('carousel-item-2'),
        },
        {
            position: 2,
            el: document.getElementById('carousel-item-3'),
        },
        {
            position: 3,
            el: document.getElementById('carousel-item-4'),
        },
    ];

    // options with default values
    const options = {
        defaultPosition: 1,
        interval: 3000,

        indicators: {
            activeClasses: 'bg-white dark:bg-gray-800',
            inactiveClasses:
                'bg-white/50 dark:bg-gray-800/50 hover:bg-white dark:hover:bg-gray-800',
            items: [
                {
                    position: 0,
                    el: document.getElementById('carousel-indicator-1'),
                },
                {
                    position: 1,
                    el: document.getElementById('carousel-indicator-2'),
                },
                {
                    position: 2,
                    el: document.getElementById('carousel-indicator-3'),
                },
                {
                    position: 3,
                    el: document.getElementById('carousel-indicator-4'),
                },
            ],
        },

        // callback functions
        onNext: () => {
            console.log('next slider item is shown');
        },
        onPrev: () => {
            console.log('previous slider item is shown');
        },
        onChange: () => {
            console.log('new slider item has been shown');
        },
    };

    // instance options object
    const instanceOptions = {
    id: 'carousel-example',
    override: true
    };

    const carousel = new Carousel(carouselElement, items, options, instanceOptions);

    carousel.cycle();

    const $prevButton = document.getElementById('data-carousel-prev');
    const $nextButton = document.getElementById('data-carousel-next');

    $prevButton.addEventListener('click', () => {
        carousel.prev();
        console.log(carousel.items)
    });

    $nextButton.addEventListener('click', () => {
        carousel.next();
    });

  });

  </script> 