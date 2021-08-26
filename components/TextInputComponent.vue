<template>
    <view class="container">
        <text-input placeholder="Nombre" class="text-input" v-model="name"></text-input>

        <text-input placeholder="Apellido" class="text-input" v-model="surname"></text-input>

    </view>
</template>

<script>
export default {
    data() {
        return {
            name:"",
            surname:""
        }
    },
}
</script>

<style>
.container {
    margin: 5px;
}
.text-input {
    border-width: 1px;
    border-color: gray;
    border-radius: 15px;
    padding-top: 5px;
    padding-bottom: 5px;
    padding-left: 15px;
    padding-right: 15px;
    margin-top: 5px;
}
</style>