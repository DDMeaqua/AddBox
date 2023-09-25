<template>
  <div>
    <div class="px-4">
      <div class="bg-[#D9EEEC] rounded-xl text-center w-full mx-auto py-4 text-3xl mb-4">
        《 人物选择 》
      </div>
      <div class="flex flex-wrap">
        <div @click="showModal = true"><Character /></div>
        <div @click="showModal = true"><Character /></div>
        <div @click="showModal = true"><Character /></div>
        <div @click="showModal = true"><Character /></div>
        <div @click="showModal = true"><Character /></div>
      </div>
    </div>

    <!-- 模态框 -->
    <div v-show="showModal" class="fixed inset-0 flex items-center justify-center z-10">
      <div class="bg-white w-4/5 sm:w-2/3 md:w-1/2 lg:w-1/3 xl:w-1/4 p-4 rounded-xl shadow-lg">
        <h2 class="text-xl font-bold mb-4">选择了 xxx</h2>
        <p class="text-gray-500 text-sm">作者：xxx ——《书名》</p>
        <div class="text-center">
        <!-- 前往按钮，点击后导航到新页面 -->
        <router-link to="/">
          <button class="bg-green-400 text-white px-4 py-2 mt-4 rounded-lg mx-4">
            对话
          </button>
        </router-link>
        
        <!-- 取消按钮，点击后关闭模态框 -->
        <button @click="showModal = false" class="bg-gray-400 text-white px-4 py-2 mt-4 rounded-lg mx-4">
          取消
        </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import Character from "../components/Character.vue";

import { ref } from 'vue';

const showModal = ref(false);
</script>
