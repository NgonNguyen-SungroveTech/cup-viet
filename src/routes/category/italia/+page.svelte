<script>
  import { Carousel } from "flowbite-svelte";

  let hidden = true;

  export let images = [
    {
      alt: "Cosmic timetraveler",
      src: "/images/category/itali/BANNER-1-01.jpg",
      title: "cupviet.com"
    },
    {
      alt: "Cosmic timetraveler",
      src: "/images/category/taybannha/BANNER-2-01.jpg",
      title: "cupviet.com"
    }
  ];

  let data = [
    {
      id: 1,
      name: "Cúp Italia CIT_415",
      image: "/images/category/itali/CIT_415.png",
      code: "CIT_415",
    },
    {
      id: 2,
      name: "Cúp Italia CIT_810",
      image: "/images/category/itali/CIT_810.png",
      code: "CIT_810",
    },
    {
      id: 3,
      name: "Cúp Italia CIT_2312-3",
      image: "/images/category/itali/CIT_2312-3REV01.png",
      code: "CIT_2312-3",
    },
    {
      id: 4,
      name: "Cúp Italia CIT_2312",
      image: "/images/category/itali/CIT_2312.png",
      code: "CIT_2312",
    },
    {
      id: 5,
      name: "Cúp Italia CIT_2312N",
      image: "/images/category/itali/CIT_2312N.png",
      code: "CIT_2312N",
    },
    {
      id: 6,
      name: "Cúp Italia CIT_2355",
      image: "/images/category/itali/CIT_2355.png",
      code: "CIT_2355",
    },
    {
      id: 7,
      name: "Cúp Italia CIT_2363",
      image: "/images/category/itali/CIT_2363.png",
      code: "CIT_2363",
    },
    {
      id: 8,
      name: "Cúp Italia CIT_2367",
      image: "/images/category/itali/CIT_2367.png",
      code: "CIT_2367",
    },
    {
      id: 9,
      name: "Cúp Italia CIT_3267-A",
      image: "/images/category/itali/CIT_3267-A.png",
      code: "CIT_3267-A",
    },
    {
      id: 10,
      name: "Cúp Italia CIT_3267-B",
      image: "/images/category/itali/CIT_3267-B.png",
      code: "CIT_3267-B",
    },
    {
      id: 11,
      name: "Cúp Italia CIT_3267",
      image: "/images/category/itali/CIT_3267.png",
      code: "CIT_3267",
    },
    {
      id: 12,
      name: "Cúp Italia CIT_3274",
      image: "/images/category/itali/CIT_3274.png",
      code: "CIT_3274",
    },
    {
      id: 13,
      name: "Cúp Italia CIT_3275",
      image: "/images/category/itali/CIT_3275.png",
      code: "CIT_3275",
    },
    {
      id: 14,
      name: "Cúp Italia CIT_3283",
      image: "/images/category/itali/CIT_3283.png",
      code: "CIT_3283",
    },
    {
      id: 15,
      name: "Cúp Italia CIT_3300",
      image: "/images/category/itali/CIT_3300.png",
      code: "CIT_3300",
    },
    {
      id: 16,
      name: "Cúp Italia CIT_3303",
      image: "/images/category/itali/CIT_3303.png",
      code: "CIT_3303",
    },
    {
      id: 17,
      name: "Cúp Italia CIT_6320",
      image: "/images/category/itali/CIT_6320.png",
      code: "CIT_6320",
    },
    {
      id: 18,
      name: "Cúp Italia CIT_7102",
      image: "/images/category/itali/CIT_7102.png",
      code: "CIT_7102",
    },
    {
      id: 19,
      name: "Cúp Italia CIT_7103",
      image: "/images/category/itali/CIT_7103.png",
      code: "CIT_7103",
    },
    {
      id: 20,
      name: "Cúp Italia CIT_7172",
      image: "/images/category/itali/CIT_7172.png",
      code: "CIT_7172",
    },
    {
      id: 21,
      name: "Cúp Italia CIT_8005",
      image: "/images/category/itali/CIT_8005.png",
      code: "CIT_8005",
    },
    {
      id: 22,
      name: "Cúp Italia CIT_8121",
      image: "/images/category/itali/CIT_8121.png",
      code: "CIT_8121",
    },
    {
      id: 23,
      name: "Cúp Italia CIT_8121G",
      image: "/images/category/itali/CIT_8121G.png",
      code: "CIT_8121G",
    },
    {
      id: 24,
      name: "Cúp Italia CIT_8121R",
      image: "/images/category/itali/CIT_8121R.png",
      code: "CIT_8121R",
    },
    {
      id: 25,
      name: "Cúp Italia CIT_9215",
      image: "/images/category/itali/CIT_9215.png",
      code: "CIT_9215",
    },
    {
      id: 26,
      name: "Cúp Italia CIT_9217",
      image: "/images/category/itali/CIT_9217.png",
      code: "CIT_9217",
    },
    {
      id: 27,
      name: "Cúp Italia CIT_9329",
      image: "/images/category/itali/CIT_9329.png",
      code: "CIT_9329",
    },
    {
      id: 28,
      name: "Cúp Italia CIT_9329N",
      image: "/images/category/itali/CIT_9329N.png",
      code: "CIT_9329N",
    },
    {
      id: 29,
      name: "Cúp Italia CIT_9380G",
      image: "/images/category/itali/CIT_9380G.png",
      code: "CIT_9380G",
    },
    {
      id: 30,
      name: "Cúp Italia CIT_16380-1N",
      image: "/images/category/itali/CIT_16380-1N.png",
      code: "CIT_16380-1N",
    },
    {
      id: 31,
      name: "Cúp Italia CIT_16380",
      image: "/images/category/itali/CIT_16380.png",
      code: "CIT_16380",
    },
    {
      id: 32,
      name: "Cúp Italia CIT_16410",
      image: "/images/category/itali/CIT_16410.png",
      code: "CIT_16410",
    },
    {
      id: 33,
      name: "Cúp Italia CIT_16540",
      image: "/images/category/itali/CIT_16540.png",
      code: "CIT_16540",
    },
    {
      id: 34,
      name: "Cúp Italia CIT_16640G",
      image: "/images/category/itali/CIT_16640G.png",
      code: "CIT_16640G",
    },
    {
      id: 35,
      name: "Cúp Italia CIT_18400-01",
      image: "/images/category/itali/CIT_18400-01.png",
      code: "CIT_18400-01",
    },
    {
      id: 36,
      name: "Cúp Italia CIT_20650",
      image: "/images/category/itali/CIT_20650.png",
      code: "CIT_20650",
    },
    {
      id: 37,
      name: "Cúp Italia CIT_20700",
      image: "/images/category/itali/CIT_20700.png",
      code: "CIT_20700",
    },
    {
      id: 38,
      name: "Cúp Italia CIT_20700G",
      image: "/images/category/itali/CIT_20700G.png",
      code: "CIT_20700G",
    },
    {
      id: 39,
      name: "Cúp Italia CIT_20750-G",
      image: "/images/category/itali/CIT_20750-G.png",
      code: "CIT_20750-G",
    },
    {
      id: 40,
      name: "Cúp Italia CIT_20750-GG",
      image: "/images/category/itali/CIT_20750-GG.png",
      code: "CIT_20750-GG",
    },
    {
      id: 41,
      name: "Cúp Italia CIT_20750",
      image: "/images/category/itali/CIT_20750.png",
      code: "CIT_20750",
    },
    {
      id: 42,
      name: "Cúp Italia CIT_20750G",
      image: "/images/category/itali/CIT_20750G.png",
      code: "CIT_20750G",
    },
    {
      id: 43,
      name: "Cúp Italia CIT_22170-1REV01",
      image: "/images/category/itali/CIT_22170-1REV01.png",
      code: "CIT_22170-1REV01",
    },
    {
      id: 44,
      name: "Cúp Italia CIT_22170",
      image: "/images/category/itali/CIT_22170.png",
      code: "CIT_22170",
    },
    {
      id: 45,
      name: "Cúp Italia CIT_22170N",
      image: "/images/category/itali/CIT_22170N.png",
      code: "CIT_22170N",
    },
    {
      id: 46,
      name: "Cúp Italia CIT_22170N",
      image: "/images/category/itali/CIT_22170N.png",
      code: "CIT_22170N",
    },
    {
      id: 47,
      name: "Cúp Italia CIT_SO-312",
      image: "/images/category/itali/CIT_SO-312.png",
      code: "CIT_SO-312",
    },
  ];
</script>

<div class="w-full text-center mt-10">
  <p
    class="sm:text-5xl text-2xl sm:mt-0 mt-10 font-medium uppercase text-yellow-400"
  >
    Cúp Italia
  </p>
  <div class="sm:grid sm:grid-cols-12 gap-4 mt-10">
    <div class="col-span-6 relative bg-slate-50 rounded-sm">
      <div
        class="absolute sm:w-16 sm:h-16 h-12 w-12 sm:p-2 bg-red-500 text-white sm:font-semibold rounded-sm"
      >
        <p>Best</p>
        <p>1</p>
      </div>
      <img
        on:mouseover={() => (hidden = false)}
        src="/images/category/itali/CIT_3275.png"
        class="sm:max-w-[600px] max-w-[400px] mx-auto"
        alt=""
      />
      {#if !hidden} 
        <div class="absolute top-0 left-0 h-full w-full bg-black opacity-65 z-50">
        </div>
        <div class='absolute top-0 left-0 font-bold w-full h-full z-[52] flex justify-center items-center' on:mouseout={() => (hidden = true)}>
          <div class="text-white">
            <p class="font-bold text-2xl">CIT_3275</p><br/>
            <p>Cúp kim loại cao cấp</p>
          </div>
        </div>
      {/if}
    </div>
    <div class="col-span-6 sm:mt-0 mt-10">
      <div class="grid grid-cols-12 gap-4">
        <div class="relative col-span-6 bg-slate-50 rounded-sm">
          <div
            class="absolute sm:w-12 sm:h-12 h-10 w-10 p-2 bg-red-500 text-white sm:font-semibold rounded-sm"
          >
            <p>2</p>
          </div>
          <img
            src="/images/category/itali/CIT_3274.png"
            class="sm:max-w-[300px] max-w-[200px] mx-auto"
            alt=""
          />
        </div>
        <div class="relative col-span-6 bg-slate-50 rounded-sm">
          <div
            class="absolute sm:w-12 sm:h-12 h-10 w-10 p-2 bg-red-500 text-white sm:font-semibold rounded-sm"
          >
            <p>3</p>
          </div>
          <img
            src="/images/category/itali/CIT_3283.png"
            class="sm:max-w-[300px] max-w-[200px] mx-auto"
            alt=""
          />
        </div>
        <div class="relative col-span-6 bg-slate-50 rounded-sm">
          <div
            class="absolute sm:w-12 sm:h-12 h-10 w-10 p-2 bg-red-500 text-white sm:font-semibold rounded-sm"
          >
            <p>4</p>
          </div>
          <img
            src="/images/category/itali/CIT_9215.png"
            class="sm:max-w-[300px] max-w-[200px] mx-auto"
            alt=""
          />
        </div>
        <div class="relative col-span-6 bg-slate-50 rounded-sm">
          <div
            class="absolute sm:w-12 sm:h-12 h-10 w-10 p-2 bg-red-500 text-white sm:font-semibold rounded-sm"
          >
            <p>5</p>
          </div>
          <img
            src="/images/category/itali/CIT_9329.png"
            class="sm:max-w-[300px] max-w-[200px] mx-auto"
            alt=""
          />
        </div>
      </div>
    </div>
  </div>

  <div class="sm:max-w-[1200px] sm:!max-h-[250px] max-h-[100px] my-10">
      <Carousel
        class="rounded-md sm:max-h-[250px] max-h-[100px]"
        {images}
        duration="3000"
      />
  </div>
  <div class="grid grid-cols-12 sm:gap-5">
    {#each data as item}
      <div
        class="sm:col-span-4 col-span-6 text-center sm:max-w-[400px] max-w-[200px]"
      >
        <img src={item.image} class="sm:max-w-[400px] max-w-[200px] bg-gray-100" alt="" />
        <div class="sm:text-2xl text-sm font-bold text-[#fcbd48] sm:px-0 flex w-full gap-2 justify-center">
          {item.code}
        </div>
        <p class="sm:text-2xl text-sm sm:px-0">
          Cúp kim loại cao cấp
        </p>
        <a class="hover:text-yellow-400 sm:text-base text-sm" href="/"
          >Xin liên hệ...</a
        >
      </div>
    {/each}
  </div>
</div>
