<template>
    <div>
        <input type="text" :value="age" @input="onAgeInput" />
        <br />
        <input type="text" :value="modelValue" @input="onSexInput" />
    </div>
</template>

<script setup>
import { defineEmits, defineProps } from "vue";
defineProps({
    age: Number,
    modelValue: String,
});
const emit = defineEmits(["age"]);
function onAgeInput(e) {
    emit("update:age", parseFloat(e.target.value));
}
function onSexInput(e) {
    emit("update:modelValue", e.target.value);
}
</script>
