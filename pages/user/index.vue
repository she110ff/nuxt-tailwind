<template>
  <div>
    <div class=" h-64 m-32 relative">
      <div class="flex flex-col items-center font-bold lg:text-6xl md:text-4xl">
        <div class="flex justify-center">
          <vue-typed-js
            :strings="['awesome', 'brilliant']"
            :loop="true"
            :typeSpeed="70"
            :backSpeed="10"
          >
            <h2 class=" text-center underline--magical">
              We make <span class="typing"></span> services.
            </h2>
          </vue-typed-js>
        </div>
        <div
          class=" text-xl md:text-lg sm:text-sm mx-auto px-20 text-center font-light"
        >
          정교하고 스타일리시한 사이트 런칭을 Earl Flex 와 함께 하세요. 웹과
          앱의 필요한 기능을 빠르게 제공합니다.
        </div>
      </div>
      <div class="flex justify-center mt-10 text-xl font-light ">
        <button
          class="bg-green-500 hover:bg-green-700 text-white py-2 px-10 rounded-full mr-4"
        >
          View Video
        </button>
        <button
          class="bg-transparent hover:bg-green-500 text-green-700  hover:text-white py-2 px-10 border border-green-500 hover:border-transparent rounded-full"
        >
          Purchase
        </button>
      </div>
    </div>

    <div class="flex flex-col items-center mt-48 p-20">
      <div class=" text-gray-500 text-sm font-medium">
        Revolutionize how you build the web and app.
      </div>
      <div class=" text-4xl font-bold">The Earl Flex Ecosystem</div>
      <div class="mt-10 w-full">
        <div class="grid lg:grid-cols-3 md:grid-cols-2 gap-6">
          <div class="flex shadow p-3">
            <div class="bg-blue-500 m-1 w-16 h-16">
              <img
                class="h-12 w-12 m-2"
                src="https://www.flaticon.com/premium-icon/icons/svg/2412/2412889.svg"
                alt=""
              />
            </div>
            <div class="ml-4 mt-5 leading-tight">
              <div class="text-lg">Vapor</div>
              <div class="text-xs font-hairline text-gray-600">
                Severless Platform
              </div>
            </div>
          </div>
          <div class="flex shadow p-3">
            <div class="bg-green-500 m-1 w-16 h-16">
              <img
                class="h-12 w-12 m-2"
                src="https://www.flaticon.com/premium-icon/icons/svg/2412/2412855.svg"
                alt="Icon"
              />
            </div>
            <div class="ml-4 mt-5 leading-tight">
              <div class="text-lg">Forge</div>
              <div class="text-xs font-hairline text-gray-600">
                Server managements
              </div>
            </div>
          </div>
          <div class="flex shadow p-3">
            <div class="bg-orange-500 m-1 w-16 h-16">
              <img
                class="h-12 w-12 m-2"
                src="https://www.flaticon.com/premium-icon/icons/svg/2412/2412854.svg"
                alt=""
              />
            </div>
            <div class="ml-4 mt-5 leading-tight">
              <div class="text-lg">Envoye</div>
              <div class="text-xs font-hairline text-gray-600">
                Auto Deployment
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.underline--magical {
  background-image: linear-gradient(120deg, #84fab0 0%, #8fd3f4 100%);
  background-repeat: no-repeat;
  background-size: 100% 0.4em;
  background-position: 0 70%;
  transition: background-size 0.25s ease-in;
  &:hover {
    background-size: 100% 88%;
  }
}

.blob {
  position: absolute;
  z-index: 0;
  transform: scale(2) rotate(170deg);
  mask-image: url("~assets/blob-2.svg");

  &.blob-2 {
    transform: scale(2) rotate(50deg);
    mask-image: url("~assets/blob.svg");
  }
  &.blob-3 {
    mask-image: url("https://jumpstart.mediumra.re/assets/img/blobs/blob-3.svg");
  }
  &.blob-4 {
    mask-image: url("https://jumpstart.mediumra.re/assets/img/blobs/blob-4.svg");
  }
  &.blob-5 {
    mask-image: url("https://jumpstart.mediumra.re/assets/img/blobs/blob-5.svg");
  }
  mask-size: 100% 100%;
  &.top {
    top: -5vw;
  }
  &.bottom {
    bottom: -5vw;
  }
  &.right {
    right: -5vw;
  }
  &.left {
    left: -5vw;
  }
}

.bg-gradient {
  background: linear-gradient(to right, #009b72, #046865) !important;
}
</style>
