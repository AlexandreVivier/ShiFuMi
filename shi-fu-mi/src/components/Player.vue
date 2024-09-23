<template>
    <div>
        <button v-on:click="rockChosen()">Pierre</button>
        <button v-on:click="paperChosen()">Feuille</button>
        <button v-on:click="scissorsChosen()">Ciseaux</button>
    </div>
</template>

<script>
export default {
    methods: {
        rockChosen() {
            this.$emit('getChoice', 'rock');
        },
        paperChosen() {
            this.$emit('getChoice', 'paper');
        },
        scissorsChosen() {
            this.$emit('getChoice', 'scissors');
        }
    }
}
</script>