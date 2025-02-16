<template>
  <div class="w-[64rem] pt-[3.875rem]">
    <div class="flex justify-between">
      <div class="w-[33.6525rem] content-center">
        <p class="font-mitr-medium text-white text-[2rem] pb-[2rem]">
          Elias is a <span class="text-primary">web designer</span> and
          <span class="text-primary">front-end developer</span>
        </p>
        <p class="font-mitr-light text-gray text-[1rem] pb-[1.5rem]">
          He crafts responsive websites where technologies meet creativity
        </p>
        <Button title="Contact me!!" />
      </div>
      <div class="relative justify-center">
        <AppSvg name="/assets/svg/home/logo.svg" class="absolute top-[3.5rem] left-[1rem]" />
        <div class="relative">
          <img
            src="/assets/png/home.png"
            class="w-[28.5625rem] h-[24.125rem]"
            alt="home"
          />
          <AppSvg
            name="/assets/svg/home/dots.svg"
            class="absolute bottom-[3.5rem] right-[1rem]"
          />
        </div>
        <div
          class="font-mitr-light text-gray text-[1rem] border border-gray p-[0.5rem] flex"
        >
          <div class="w-[1rem] h-[1rem] mr-[0.5rem] bg-primary self-center" />
          <p>Currently working on <span class="text-white">Portfolio</span></p>
        </div>
      </div>
    </div>
    <div class="relative justify-self-center p-[2rem] border border-gray mt-[7rem]">
      <div
        class="absolute px-[0.25rem] py-[0.5rem] top-[-1rem] left-[1rem] bg-background"
      >
        <AppSvg name="/assets/svg/home/quotation-mark.svg" />
      </div>
      <p class="font-mitr text-[1.5rem] text-gray">
        With great power comes great electricity bill
      </p>
      <div
        class="absolute px-[0.25rem] py-[0.5rem] bottom-[-1rem] right-[1rem] bg-background"
      >
        <AppSvg name="/assets/svg/home/quotation-mark.svg" />
      </div>
    </div>
  </div>
</template>

<script>
const onClick = () => {
  console.log("onClick");
};
</script>
