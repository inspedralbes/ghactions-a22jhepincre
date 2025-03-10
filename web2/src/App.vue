<script setup>

</script>

<script>
import { ref } from 'vue'

export default {
  setup() {
    const text = ref("");
    
    let handleClickButton = (value)=>{
      text.value = value;
    }

    return { text, handleClickButton }
  },
  template: `<div>Count is: {{ count }}</div>`
}

</script>

<template>
  <div
    class="mx-auto overflow-hidden mt-10 shadow-lg mb-2 bg-purple-900 shadow-lg border rounded-lg lg:w-2/6 md:w-3/6 sm:w-4/6">
    <div class="">
      <div class="p-5 text-white text-center text-3xl bg-purple-900"><span class="text-orange-500">Calcu</span>lator
      </div>
      <div class=" p-5 text-white text-right text-3xl bg-purple-800">{{text}}</div>

      <div class="flex items-stretch bg-purple-900 h-24">
        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(7)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            7</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(8)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            8</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(9)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            9</div>
        </div>
      </div>

      <div class="flex items-stretch bg-purple-900 h-24">
        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(4)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            4</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(5)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            5</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(6)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            6</div>
        </div>
      </div>

      <div class="flex items-stretch bg-purple-900 h-24">
        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(1)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            1</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(2)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            2</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(2)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            3</div>
        </div>
      </div>

      <div class="flex items-stretch bg-purple-900 h-24 mb-4">
        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div @click="handleClickButton(0)"
            class="rounded-full h-20 w-20 flex items-center bg-purple-800 justify-center shadow-lg border-2 border-purple-700 hover:border-2 hover:border-gray-500 focus:outline-none">
            0</div>
        </div>
      </div>
    </div>
  </div>

</template>

<style scoped></style>
