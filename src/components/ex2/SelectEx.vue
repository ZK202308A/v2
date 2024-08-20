<template>
  <div>
    <ul ref="list">
      <li v-for="{mno,title} in props.arr">
        <input type="checkbox" value="{{ mno }}" name="checkList" > {{ mno }} -- {{ title }}
      </li>
    </ul>
    <div>
      <button @click="handleClick" >REMOVE</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const list = ref(null)

const props = defineProps(['arr'])



console.log(props.arr)

const handleClick = () => {
  console.log("click")
  const ul = list.value 
  console.log(ul.querySelectorAll("li input[type='checkbox']:checked"))
}

</script>

<style lang="scss" scoped>

</style>