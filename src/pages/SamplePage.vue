<template>
<MyNav></MyNav>
<div class="container">

  <MyTilte></MyTilte>

  <TodoContainer></TodoContainer>

</div>
</template>

<script setup>
import TodoContainer from '../components/ex4/TodoContainer.vue';
import CountEx from '../components/ex3/index.vue'
import CountContainer from '../components/ex3/CountContainer.vue';
import SelectEx2 from '../components/ex2/SelectEx2.vue';
import InputEx from '../components/ex2/InputEx.vue';
import MyNav from '../components/MyNav.vue';
import MyFooter from '../components/MyFooter.vue';
import MyTilte from '../components/MyTilte.vue';
import Counter2 from '../components/ex1/Counter2.vue';
import MyContent from '../components/MyContent.vue';

import SelectEx from '../components/ex2/SelectEx.vue';

const message = {sender:'AAA', text:'BBBBB'}

const mails = [
    {mno:1, title:'AAAAA'},
    {mno:2, title:'BAAAA'},
    {mno:3, title:'CAAAA'},
    {mno:4, title:'DAAAA'},
    {mno:5, title:'EAAAA'},
]

const doA = () => {
  console.log('doA')
}

</script>

<style lang="scss" scoped>




</style>