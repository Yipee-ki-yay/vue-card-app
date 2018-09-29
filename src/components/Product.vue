<template>
    <div>
        <h2>Product title</h2>
        <div class="price">Price: {{ price }}</div>
        <hr>
        <div class="btn btn-warning" @click="minus">-1</div>
        <div class="btn btn-success" @click="plus">+1</div>
        <input type="text" v-model="cnt">
    </div>
</template>

<script>
    import {mapGetters} from 'vuex';
    import {mapMutations} from 'vuex';

    export default {
        methods: {
            ...mapMutations([
                'minus',
                'plus'
            ]),
            onInput(e) {
                
            }
        },
        computed: {
            ...mapGetters([
                'price',
            ]),
            cnt: {
                get() {
                    return this.$store.getters.cnt;
                },
                set(value) {
                    this.$store.commit('setCnt', value);
                }
            }
        }
    }
</script>

