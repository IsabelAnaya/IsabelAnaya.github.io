<script>

    import { onMount } from "svelte";
    let te;

    onMount(async () => {
        te = await import('tw-elements');
        te.initTE({ Carousel: te.Carousel });
    });
</script>

<head>
    <!-- Tailwind Elements styles. this kills the layered styles-->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tw-elements/dist/css/tw-elements.min.css" />
    <title>Projects - Isabel Anaya</title>
</head>

<body>
    <h1 class="font-extrabold text-black text-2xl">Projects</h1>
    <div class="main-card">
        <h2 class="text-white text-xl font-bold">BorkBoard</h2>
        <div id="carouselBB" class="relative" data-te-carousel-init data-te-carousel-slide>
            <!--Carousel indicators-->
            <div class="absolute bottom-0 left-0 right-0 z-[2] mx-[15%] mb-4 flex list-none justify-center p-0" data-te-carousel-indicators>
                <button
                type="button"
                data-te-target="#carouselBB"
                data-te-slide-to="0"
                data-te-carousel-active
                class="mx-[3px] box-content h-[3px] w-[30px] flex-initial cursor-pointer border-0 border-y-[10px] border-solid border-transparent bg-black bg-clip-padding p-0 -indent-[999px] opacity-50 transition-opacity duration-[600ms] ease-[cubic-bezier(0.25,0.1,0.25,1.0)] motion-reduce:transition-none"
                aria-current="true"
                aria-label="Slide 1"></button>
                <button
                type="button"
                data-te-target="#carouselBB"
                data-te-slide-to="1"
                class="mx-[3px] box-content h-[3px] w-[30px] flex-initial cursor-pointer border-0 border-y-[10px] border-solid border-transparent bg-black bg-clip-padding p-0 -indent-[999px] opacity-50 transition-opacity duration-[600ms] ease-[cubic-bezier(0.25,0.1,0.25,1.0)] motion-reduce:transition-none"
                aria-label="Slide 2"></button>
            </div>

            <!--Carousel items-->
            <div
                class="relative w-full overflow-hidden after:clear-both after:block after:content-['']">
                <!--First item-->
                <div
                class="relative float-left -mr-[100%] w-full transition-transform duration-[600ms] ease-in-out motion-reduce:transition-none"
                data-te-carousel-active
                data-te-carousel-item
                style="backface-visibility: hidden">
                <img
                    src="/media/bb_1.png"
                    class="block w-full"
                    alt="..." />
                <div
                    class="absolute inset-x-[15%] bottom-5 hidden py-5 text-center text-white md:block">
                    <p></p>
                </div>
                </div>
                <!--Second item-->
                <div
                class="relative float-left -mr-[100%] hidden w-full transition-transform duration-[600ms] ease-in-out motion-reduce:transition-none"
                data-te-carousel-item
                style="backface-visibility: hidden">
                    <!-- svelte-ignore a11y-img-redundant-alt -->
                    <img
                        src="/media/bb_2.png"
                        class="block w-full"
                        alt="..." />
                    <div class="absolute inset-x-[15%] bottom-5 hidden py-5 text-center text-white md:block">
                        <p></p>
                    </div>
                </div>
            </div>

            <!--Carousel controls - prev item-->
            <button
                class="absolute bottom-0 left-0 top-0 z-[1] flex w-[15%] items-center justify-center border-0 bg-none p-0 text-center text-black opacity-50 transition-opacity duration-150 ease-[cubic-bezier(0.25,0.1,0.25,1.0)] hover:text-black hover:no-underline hover:opacity-90 hover:outline-none focus:text-black focus:no-underline focus:opacity-90 focus:outline-none motion-reduce:transition-none"
                type="button"
                data-te-target="#carouselBB"
                data-te-slide="prev">
                <span class="inline-block h-8 w-8">
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="h-6 w-6">
                    <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M15.75 19.5L8.25 12l7.5-7.5" />
                </svg>
                </span>
                <span
                class="!absolute !-m-px !h-px !w-px !overflow-hidden !whitespace-nowrap !border-0 !p-0 ![clip:rect(0,0,0,0)]"
                >Previous</span
                >
            </button>
            <!--Carousel controls - next item-->
            <button
                class="absolute bottom-0 right-0 top-0 z-[1] flex w-[15%] items-center justify-center border-0 bg-none p-0 text-center text-black opacity-50 transition-opacity duration-150 ease-[cubic-bezier(0.25,0.1,0.25,1.0)] hover:text-black hover:no-underline hover:opacity-90 hover:outline-none focus:text-black focus:no-underline focus:opacity-90 focus:outline-none motion-reduce:transition-none"
                type="button"
                data-te-target="#carouselBB"
                data-te-slide="next">
                <span class="inline-block h-8 w-8">
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="h-6 w-6">
                    <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
                </span>
                <span
                class="!absolute !-m-px !h-px !w-px !overflow-hidden !whitespace-nowrap !border-0 !p-0 ![clip:rect(0,0,0,0)]"
                >Next</span
                >
            </button>
        </div>
        <p>An offline bulletin board application to store and manage notes. Currently in development.</p>
        <a href="https://github.com/IsabelAnaya/borkboard" class="underline italic">Github Link</a>
    </div>
    <div class="main-card">
        <h2 class="text-white text-xl font-bold">IMAGE BREAKER</h2>
        <div id="carouselIB" class="relative" data-te-carousel-init data-te-carousel-slide>
            <!--Carousel indicators-->
            <div class="absolute bottom-0 left-0 right-0 z-[2] mx-[15%] mb-4 flex list-none justify-center p-0" data-te-carousel-indicators>
                <button
                type="button"
                data-te-target="#carouselIB"
                data-te-slide-to="0"
                data-te-carousel-active
                class="mx-[3px] box-content h-[3px] w-[30px] flex-initial cursor-pointer border-0 border-y-[10px] border-solid border-transparent bg-white bg-clip-padding p-0 -indent-[999px] opacity-50 transition-opacity duration-[600ms] ease-[cubic-bezier(0.25,0.1,0.25,1.0)] motion-reduce:transition-none"
                aria-current="true"
                aria-label="Slide 1"></button>
                <button
                type="button"
                data-te-target="#carouselIB"
                data-te-slide-to="1"
                class="mx-[3px] box-content h-[3px] w-[30px] flex-initial cursor-pointer border-0 border-y-[10px] border-solid border-transparent bg-white bg-clip-padding p-0 -indent-[999px] opacity-50 transition-opacity duration-[600ms] ease-[cubic-bezier(0.25,0.1,0.25,1.0)] motion-reduce:transition-none"
                aria-label="Slide 2"></button>
            </div>

            <!--Carousel items-->
            <div
                class="relative w-full overflow-hidden after:clear-both after:block after:content-['']">
                <!--First item-->
                <div
                class="relative float-left -mr-[100%] w-full transition-transform duration-[600ms] ease-in-out motion-reduce:transition-none"
                data-te-carousel-active
                data-te-carousel-item
                style="backface-visibility: hidden">
                <img
                    src="/media/imgbrkr.png"
                    class="block w-full"
                    alt="..." />
                <div
                    class="absolute inset-x-[15%] bottom-5 hidden py-5 text-center text-white md:block">
                    <p>IMAGE BREAKER's interface.</p>
                </div>
                </div>
                <!--Second item-->
                <div
                class="relative float-left -mr-[100%] hidden w-full transition-transform duration-[600ms] ease-in-out motion-reduce:transition-none"
                data-te-carousel-item
                style="backface-visibility: hidden">
                    <!-- svelte-ignore a11y-img-redundant-alt -->
                    <img
                        src="/media/imgbrkr_1.png"
                        class="block w-full"
                        alt="..." />
                    <div class="absolute inset-x-[15%] bottom-5 hidden py-5 text-center text-white md:block">
                        <p>Example output.</p>
                    </div>
                </div>
            </div>

            <!--Carousel controls - prev item-->
            <button
                class="absolute bottom-0 left-0 top-0 z-[1] flex w-[15%] items-center justify-center border-0 bg-none p-0 text-center text-white opacity-50 transition-opacity duration-150 ease-[cubic-bezier(0.25,0.1,0.25,1.0)] hover:text-white hover:no-underline hover:opacity-90 hover:outline-none focus:text-white focus:no-underline focus:opacity-90 focus:outline-none motion-reduce:transition-none"
                type="button"
                data-te-target="#carouselIB"
                data-te-slide="prev">
                <span class="inline-block h-8 w-8">
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="h-6 w-6">
                    <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M15.75 19.5L8.25 12l7.5-7.5" />
                </svg>
                </span>
                <span
                class="!absolute !-m-px !h-px !w-px !overflow-hidden !whitespace-nowrap !border-0 !p-0 ![clip:rect(0,0,0,0)]"
                >Previous</span
                >
            </button>
            <!--Carousel controls - next item-->
            <button
                class="absolute bottom-0 right-0 top-0 z-[1] flex w-[15%] items-center justify-center border-0 bg-none p-0 text-center text-white opacity-50 transition-opacity duration-150 ease-[cubic-bezier(0.25,0.1,0.25,1.0)] hover:text-white hover:no-underline hover:opacity-90 hover:outline-none focus:text-white focus:no-underline focus:opacity-90 focus:outline-none motion-reduce:transition-none"
                type="button"
                data-te-target="#carouselIB"
                data-te-slide="next">
                <span class="inline-block h-8 w-8">
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="h-6 w-6">
                    <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
                </span>
                <span
                class="!absolute !-m-px !h-px !w-px !overflow-hidden !whitespace-nowrap !border-0 !p-0 ![clip:rect(0,0,0,0)]"
                >Next</span
                >
            </button>
        </div>
        <p>A program to glitch images through random bit shifts.</p>
        <a href="https://github.com/IsabelAnaya/image-breaker" class="underline italic">Github Link</a>
    </div>
</body>