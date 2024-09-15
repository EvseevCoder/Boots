<template>
    <div class="relative bg-white border border-slate-100 rounded-3xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl">
        <img
            class="absolute top-8 left-8"
            :src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
            @click="onClickFavorite"
            alt="Like"
        >
        <img
            :src="imageUrl"
            alt=""
        >
        <p class="mt-2">{{ title }}</p>

        <div class="flex justify-between mt-5">
            <div class="flex flex-col">
                <span class="text-slate-400">Цена: </span>
                <b>{{ price }} руб.</b>
            </div>

            <img
                :src="isAdded ? '/checked.svg' : '/plus.svg'"
                @click="onClickAdd"
                alt="Plus"
            >
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