<template>
    <li class="text">{{ todo.text }}</li>
</template>

<script type="text/ecmascript-6">
    export default {
        props: ['todo'],
    }
</script>

<style>
.text {
    color: green;
}
</style>