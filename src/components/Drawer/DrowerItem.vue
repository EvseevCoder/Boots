<template>
    <div class="flex items-center border border-slate-100 p-4 rounded-xl gap-4">
        <img
            class="w-16 h-16"
            :src="imageUrl"
            alt=""
        >

        <div class="flex flex-col">
            <p> {{ title }}</p>

            <div class="flex justify-between mt-2">
                <b> {{ price }} руб.</b>
                <img
                    class="opacity-40 hover:opacity-100 cursor-pointer transition"
                    src="/close.svg"
                    alt=""
                >
            </div>
        </div>
    </div>
</template>

<script setup>
    defineProps({
        title: {type: String, default: 'Мужские кроссовки Nike'},
        imageUrl: {type: String, default: '/sneakers/sneakers-1.jpg'},
        price: {type: Number, default: 0},
        isFavorite: {type: Boolean, default: false},
        isAdded: {type: Boolean, default: false},
        onClickAdd: {type: Function},
        onClickFavorite: {type: Function},
    });
</script>