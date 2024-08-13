<template>
    <header class="flex justify-between border-b border-slate-200 px-8 py-8">
        <div class="flex items-center gap-4">
            <img
                class="w-10"
                src="/logo.png"
                alt="Logo"
            >
            <div>
                <h2 class="text-xl font-bold uppercase">Vue Boots</h2>
                <p class="text-slate-400">Магазин Лучших кроссовок</p>
            </div>
        </div>

        <ul class="flex items-center gap-10">
            <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
                <img
                    src="/cart.svg"
                    alt="cart"
                >
                <b>1205 руб.</b>
            </li>

            <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
                <img
                    src="/heart.svg"
                    alt="cart"
                >
                <span>Закладки</span>
            </li>
            <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
                <img
                    src="/profile.svg"
                    alt="cart"
                >
                <span>Профиль</span>
            </li>
        </ul>
    </header>
</template>