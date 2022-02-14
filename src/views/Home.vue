<template>
    <div class="home">
        {{age02}} {{sex02}}
        <compositionapi
            v-model="sex02"
            v-model:age="age02"
            @test="getData"
            :keywords="keywords"
        ></compositionapi>
    </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";
import compositionapi from "@/components/HelloWorld.vue";

let age02 = ref(1111);
let sex02 = ref("nan");
</script>
