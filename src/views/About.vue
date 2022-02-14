<template>
    <div class="about">
        <h1>{{ msg }}</h1>
    </div>
</template>
<script lang="ts" setup>
let msg: unknown = "为什么啊";

function createArray<T = string>(length: number, value: T): Array<T> {
    let result: T[] = [];
    for (let i = 0; i < length; i++) {
        result[i] = value;
    }
    return result;
}
</script>
