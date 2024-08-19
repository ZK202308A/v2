<template>
    <div class="row g-3" >
        <div class="col-md-6 col-lg-4 col-xl-3" v-for="({pno,pname,price,sale}) in arr" :key="pno">
            <h2>{{ pname }}</h2>
            <p>{{price}} HTML is the standard markup language for describing the structure of the web pages. Our HTML tutorials will help you to understand the basics of latest HTML5 language, so that you can create your own website.</p>
            <p><a href="https://www.tutorialrepublic.com/html-tutorial/" target="_blank" class="btn btn-success">Learn More &raquo;</a></p>
        </div>
    </div>
</template>

<script setup>

const arr = [
    {pno: 1, pname:'P1', price: 3000, sale: true},
    {pno: 2, pname:'P2', price: 4000, sale: false},
    {pno: 3, pname:'P3', price: 5000, sale: true},
    {pno: 4, pname:'P4', price: 6000, sale: false},
]



</script>

<style lang="scss" scoped>

</style>