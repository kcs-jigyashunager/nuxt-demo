<template>
    <div>
        <h2>About</h2>
        <div>
            {{ data }}
        </div>
    </div>
</template>

<script setup>
    const { data } = await useFetch('api/ninja?name=mario')
</script>

<style scoped>
    h2 {
        margin-bottom: 20px;
        font-size: 36px;
    }
</style>