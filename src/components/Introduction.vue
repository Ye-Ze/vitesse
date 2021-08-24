<script setup lang="ts">
const keys = ['英文姓名', '個人資料', '就業狀態', 'E-mail']
const info = { '中文姓名': '林曄澤', '英文姓名': 'Ye-Ze Lin', '個人資料': '男、84年次', '就業狀態': '就業中', 'E-mail': 'otaku84334@gmail.com' }
const skill = ['C#', 'python', 'django', 'HTML', 'CSS', 'javascript', 'jQuery', 'MySQL']
</script>

<template>
  <div
    class="text-left leading-loose sticky top-0 left-0"
    p="4"
  >
    <div>
      <div>
        <img
          src="data:image/jpg;base64,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"
          alt="photo"
          class="rounded-full"
          m="x-auto y-4"
          w="40"
          h="40"
        />
      </div>
    </div>
    <br>
    <div
      text="2xl left"
      font="semibold"
      m="b-4"
    >
      {{ info.中文姓名 }}
    </div>
    <div m="b-4">
      <div
        v-for="lang in skill"
        :key="lang"
        class="inline-block"
        opacity="100"
        rounded="full"
        bg="gray-700"
        text="light-500 bold xs"
        dark:bg="light-700"
        dark:text="dark-500"
        m="x-2"
        p="y-1 x-2"
      >
        {{ lang }}
      </div>
    </div>
    <div class="grid-rows-4">
      <div
        v-for="key in keys"
        :key="key"
        class="grid grid-cols-12"
      >
        <div class="col-span-4 break-words" font="semibold">
          {{ key }}
        </div>
        <div class="col-span-8">
          {{ info[key] }}
        </div>
      </div>
    </div>
  </div>
</template>
