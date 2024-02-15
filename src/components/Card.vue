<script setup lang="ts">
import { defineProps } from 'vue';
import {GENDER, type Invitee} from '../types'

defineProps<{
    invitee: Invitee
}>()
</script>

<template>
    <div :style="{background: invitee.gender == GENDER.MALE ? 'rgb(8, 111,111)' : 'rgb(111,18,8)'}">
        {{ invitee.name }}
    </div>
</template>

<style scoped>

div {
    border-radius: 5px;
    margin-top: 5px;
    text-align: center;
    padding: 3px;
    color: white;
    background-color: aqua;
}
</style>
