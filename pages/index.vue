<template>
    <MainLayout>
        <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2">
            <div v-if="products" class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4">
                <div v-for="product in products" :key="product">
                    <ProductComponent :product="product"/>
                </div>
            </div>
        </div>
    </MainLayout>
</template>
<script setup>
import MainLayout from '~/layouts/MainLayout.vue';

let products = ref(null);

 products = [
    {id: 1, title: "Title 1", description: "", url:"https://picsum.photos/id/212/800/800", price: 9899},
    {id: 2, title: "Title 2", description: "", url:"https://picsum.photos/id/212/800/800", price: 9899},
    {id: 3, title: "Title 3", description: "", url:"", price: 9899},
    {id: 4, title: "Title 4", description: "", url:"", price: 9899},
    {id: 5, title: "Title 5", description: "", url:"", price: 9899},
    {id: 6, title: "Title 6", description: "", url:"", price: 9899},
    {id: 7, title: "Title 7", description: "", url:"", price: 9899},
    {id: 8, title: "Title 8", description: "", url:"", price: 9899},
    {id: 9, title: "Title 9", description: "", url:"", price: 9899},
    {id: 10, title: "Title 10", description: "", url:"", price: 9899},
];

</script>