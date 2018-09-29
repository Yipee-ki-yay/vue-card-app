<template>
    <div>
        <h2>Product title</h2>
        <div class="price">1000</div>
        <hr>
        <div class="btn btn-warning" @click="onMinus">-1</div>
        <div class="btn btn-success" @click="onPlus">+1</div>
    </div>
</template>

<script>
    export default {
        methods: {
            onMinus() {
                this.$emit('minus');
            },
            onPlus() {
                this.$emit('plus');
            }
        },
        computed: {
            
        }
    }
</script>

