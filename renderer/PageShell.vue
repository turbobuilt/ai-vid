<template>
    <div class="layout">
        <div class="navigation">
            Nav
        </div>
        <div class="content">
            <slot />
        </div>
    </div>
</template>

<script lang="ts" setup>
import Link from './Link.vue'
</script>

<style>
body {
    margin: 0;
    font-family: sans-serif;
}
* {
    box-sizing: border-box;
}
a {
    text-decoration: none;
}
</style>

<style scoped>
.layout {
    display: flex;
    flex-direction: column;
}
.content {
    padding: 20px;
    border-left: 2px solid #eee;
    padding-bottom: 50px;
}
.navigation {
    padding: 20px;
    flex-shrink: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    line-height: 1.8em;
}
.logo {
    margin-top: 20px;
    margin-bottom: 10px;
}
</style>
