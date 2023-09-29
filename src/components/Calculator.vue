<template>
    <div class="container mt-5">
        <input v-model="num1" type="number" placeholder="Enter a number" />
        <input v-model="num2" type="number" placeholder="Enter another number" />
        <br>
        <button class="mt-3" @click="add">Add</button>
        <button @click="subtract">Subtract</button>
        <button @click="multiply">Multiply</button>
        <button class="mb-3" @click="divide">Divide</button>
        <div class="h6">
            Result: {{ result }}
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            num1: 0,
            num2: 0,
            result: 0,
        };
    },
    methods: {
        add() {
            this.result = this.num1 + this.num2;
        },
        subtract() {
            this.result = this.num1 - this.num2;
        },
        multiply() {
            this.result = this.num1 * this.num2;
        },
        divide() {
            this.result = this.num1 / this.num2;
        },
    },
};
</script>