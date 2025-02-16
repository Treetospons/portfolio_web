<template>
  <div class="flex mt-[6.625rem] mb-[0.75rem] justify-between">
    <div class="flex">
      <h1 class="font-mitr text-[2rem] text-white">
        <span class="text-primary">#</span>about-me
      </h1>
      <span
        class="w-[14.9375rem] h-[0.0625rem] border border-primary self-center ml-[1rem]"
      />
    </div>
  </div>
  <div class="flex justify-between mt-[1.5rem]">
    <div class="w-[32.1875rem]">
      <p class="font-mitr-light text-[1rem] text-gray">
        Hello, i’m Elias!
      </p>
      <p class="font-mitr-light text-[1rem] text-gray mt-[1rem]">
        I’m a self-taught front-end developer based in Kyiv, Ukraine. I
        can develop responsive websites from scratch and raise them into modern
        user-friendly web experiences. 
      </p>
      <p class="font-mitr-light text-[1rem] text-gray mt-[1rem]">
        Transforming my creativity and knowledge into a
        websites has been my passion for over a year. I have been helping various clients
        to establish their presence online. I always strive to learn about the newest
        technologies and frameworks.
      </p>
      <Button title="Read more ->" class="mt-[1.5rem]"/>
    </div>
    <div class="relative w-[21.1875rem] justify-center">
      <AppSvg
        name="/assets/svg/home/dots.svg"
        class="absolute top-[3.5rem] left-[1rem]"
      />
      <div class="relative border-b border-b-gray">
        <img
          src="/assets/png/about-me/profile.png"
          class="h-[31.6875rem]"
          alt="profile"
        />
        <AppSvg
          name="/assets/svg/home/dots.svg"
          class="absolute bottom-[3.5rem] right-[1rem]"
        />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style></style>
