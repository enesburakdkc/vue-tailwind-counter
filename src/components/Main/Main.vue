<script setup>
import { ref } from 'vue';

const count = ref(0);

const increase = () => {
    count.value++;
}

const decrease = () => {
    count.value--;
}

const reset = () => {
    count.value = 0;
}
</script>

<template>
    <main>
        <h1 class="font-semibold">Counter</h1>

        <p class="text-5xl h-48 flex justify-center items-center">{{ count }}</p>

        <div class="flex flex-row gap-4">
            <button @click="decrease">Decrease</button>
            <button @click="reset">Reset</button>
            <button @click="increase">Increase</button>
        </div>
    </main>
</template>

<style scoped></style>