<template>
    <div class="grid mt-8 grid-cols-4 gap-5">
        <Cart
            v-for="item in items"
            :key="item.id"
            :title="item.title"
            :price="item.price"
            :imageUrl="item.imageUrl"
        />
    </div>
</template>

<script setup>
    import Cart from './Cart.vue';

    defineProps({items: Array});
</script>