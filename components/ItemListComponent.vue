<template>
    <view class="card" >
        <text>
            {{ title }}
        </text>
    </view>
</template>


<script>
export default {
    props: {
        title: {
            type: String,
            //default: "Sin Valor!"
            required: true
        }
    }
}
</script>

<style>
.card {
    width: 100%;
    border-width: 1px;
    border-color: gray;
    border-radius: 15px;
    margin-bottom: 15px;
    background-color: #FFFFFF;
    padding: 15px;
}
</style>