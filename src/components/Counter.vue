<template>
  <main class="p-4 h-screen bg-gray-700">
    <header class="text-center leading-none">
      <h1 class="text-4xl text-gray-400 font-mono font-semibold tracking-wide">
        <slot></slot>
      </h1>
      <p class="text-gray-800">increase the counter, as you like</p>
    </header>
    <section class="max-w-xxs mx-auto mt-8 flex justify-between items-center text-3xl text-gray-400">
      <button @click="value1 += 1" type="button" class="block w-16 h-24 text-center rounded-sm border border-gray-800 hover:border-gray-400 focus:outline-none focus:border-gray-400">{{ value1 }}</button>
      <button @click="value2 += 1" type="button" class="block w-16 h-24 text-center rounded-sm border border-gray-800 hover:border-gray-400 focus:outline-none focus:border-gray-400">{{ value2 }}</button>
      <button @click="value3 += 1" type="button" class="block w-16 h-24 text-center rounded-sm border border-gray-800 hover:border-gray-400 focus:outline-none focus:border-gray-400">{{ value3 }}</button>
    </section>
  </main>
</template>

<script>
export default {
  data: () => {
    return {
      value1: 0,
      value2: 0,
      value3: 0
    };
  }
};
</script>

<style>
  .max-w-xxs {
    max-width: 16rem;
  }

</style>
