<template>
    <div class="container">
        <button v-on:click="newGame()"> Recommencer la partie </button>
    </div>
</template>

<script>
export default {
    methods: {
        newGame() {
            this.$emit('newGame');
        }
    }
}
</script>