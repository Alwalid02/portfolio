<script setup>
definePageMeta({
    layout: 'products'
})

//fetch the product
const{ data: products } = await useFetch('https://fakestoreapi.com/products/')

</script>

<template>
    <div>
        <div class="grid grid-cols-4 gap-5 mt-8 mb-8">
            <div v-for="p in products">
                <product-card :product="p"/>
            </div>
        </div>
    </div>
</template>