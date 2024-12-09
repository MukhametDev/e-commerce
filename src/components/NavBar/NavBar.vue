<script setup lang="ts"></script>
<template>
    <div class="bg-dark-blue w-[100%] text-white py-[12px]">
        <div class="max-w-[1200px] m-auto flex justify-between ">
            <div class="text-white flex gap-[10px]">
                <div class="relative flex flex-col justify-between w-[24px] h-[24px] py-[2px]">
                    <div class="dots relative z-50 flex justify-center w-[24px] h-[4px]">
                        <div
                            class="w-[4px] h-[4px] rounded-[50px] bg-white transition-all duration-300 ease-in-out z-100">
                        </div>
                    </div>
                    <div class="dots relative z-50 flex justify-center w-[24px] h-[4px]">
                        <div class="w-[4px] h-[4px] rounded-[50px] bg-white transition-all duration-300 ease-in-out">
                        </div>
                    </div>
                    <div class="dots relative z-50 flex justify-center w-[24px] h-[4px]">
                        <div class="w-[4px] h-[4px] rounded-[50px] bg-white transition-all duration-300 ease-in-out">
                        </div>
                    </div>
                </div>
                <span class="">Каталог товаров</span>
            </div>

            <div class="">
                <input type="text">
            </div>
            <div class=""></div>
            <div class=""></div>
        </div>
    </div>
</template>

<style>
.dots::before{
    left: 0;
    width: 4px;
    height: 4px;
}
.dots::after{
    right: 0;
    width: 4px;
    height: 4px;
}
.dots::before,
.dots::after {
    color: white;
    content: '';
    display: block;
    position: absolute;
    border-radius: 50px;
    background-color: white;
    transition: all 0.3s ease-in-out;
    z-index: 100;
}
</style>
