<template>
  <div>
    <div class="pt-4">
      <router-link to="/">
        <img
          class="w-16 h-16 rounded-full mx-auto border"
          src="/hhh.png"
          alt=""
        />
      </router-link>
      <h3 class="text-center mt-4">用户名</h3>
      <div class="text-center mt-4">
        <button
          class="text-white bg-gradient-to-r from-blue-400 via-blue-400 to-blue-400 hover:bg-gradient-to-br focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-3xl text-sm px-8 py-2 text-center"
        >
          关注
        </button>
      </div>
    </div>

    <Answer
      title="开学焦虑怎么办"
      content="找我吃饭!我感觉我没有开学焦虑的很大一部分原因是因为一开学就可以见到两个月没见的好朋友们啦"
    />

    <!-- 其他 -->

    <router-link to="/info">
      <Card
        title="为什么要睡着"
        userimg="/hhh.png"
        content="缺乏睡眠会死人的"
      />
    </router-link>

    <router-link to="/info">
      <Card
        title="暑假怎么找相关专业的实习呀😐"
        userimg="/hhh.png"
        content="海投，去招聘软件"
      />
    </router-link>
  </div>
</template>

<script setup>
import Answer from "../components/Answer.vue";
import Card from "../components/Card.vue";
</script>
