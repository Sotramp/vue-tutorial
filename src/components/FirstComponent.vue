<template>
    <div>
        <span>Hello {{ msg }}</span>
        <p>Test de la fonction : {{ onlyFirstWord }}</p>
    </div>
</template>

<script>
export default {
    data(){
        return {
            msg: "World test",
        }
    },
    computed: {
        onlyFirstWord(){
            return this.msg.split(' ')[0].toUpperCase();
        }
    }
}
</script>

<style>

</style>