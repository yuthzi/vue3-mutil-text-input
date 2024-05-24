<script setup lang="ts">
import MutilTextInput from './components/MutilTextInput/src/MutilTextInput.vue'
import MultiTextInputItem from './components/MutilTextInput/src/components/MultiTextInputItem.vue'
</script>

<template>
  <main>
    <div class="wrapper">
      <MutilTextInput
        name="item-input"
        :values="[{ data: 'a' }, { data: 'b' }, { data: 'c' }]"
        :label="`尺寸`"
        :placeholder="`输入任意字符，每个元素之间用回车分割`"
      />

      <!-- <MultiTextInputItem :val="{ data: 'a', v: 'aa' }" :dataKey="`v`" /> -->
    </div>
  </main>
</template>

<style scoped>
@media (min-width: 1024px) {
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
