<template>
  <main class="px-12 py-4 h-screen bg-gray-700">
    <header>
      <h1 class>
        <slot></slot>
      </h1>
      <p>increase the counter, as you like:</p>
    </header>
    <section class="max-w-xs flex justify-between items-center">
      <div class="w-12 h-16 border rounded-sm font-xl text-center">
        <button @click="value1 += 1" class="block h-full w-full" type="button">{{ value1 }}</button>
      </div>
      <div class="w-12 h-16 border rounded-sm font-xl text-center">
        <button @click="value2 += 1" class="block h-full w-full" type="button">{{ value2 }}</button>
      </div>
      <div class="w-12 h-16 border rounded-sm font-xl text-center">
        <button @click="value3 += 1" class="block h-full w-full" type="button">{{ value3 }}</button>
      </div>
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
