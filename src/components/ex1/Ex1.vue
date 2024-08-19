
<template>
  <div>
    <h1>Ex1</h1>

    <div v-text="str"></div>
    
    <div>{{ str }}</div>

    <div v-html="str"></div>


    <hr/>

    {{ str ? '<h2>AAA</h2>':'<h2>BBB</h2>' }}

    <hr/>

    <template v-if="str">
      <h2>AAAA</h2>
    </template>
    <template v-else="str">
      <h2>BBBB</h2>
    </template>

    
  </div>
</template>

<script setup>

let str =  null 

</script>

<style lang="scss" scoped>

</style>