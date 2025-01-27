<script setup>
import { ref } from 'vue';

const count = ref(0);

const increase = () => {
    count.value++;
}

const decrease = () => {
    count.value--;
}
</script>

<template>
    <main class="scale-120">
        <h1>Counter</h1>

        <p class="text-4xl h-52 flex justify-center items-center">{{ count }}</p>

        <div class="flex flex-row gap-4">
            <button @click="decrease">Decrease</button>
            <button @click="increase">Increase</button>
        </div>
    </main>
</template>

<style scoped></style>