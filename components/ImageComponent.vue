<template>
    <view class="container">
        <image class="image" :source="{uri:'https://cdn.pixabay.com/photo/2021/02/10/22/13/lake-6003727_960_720.jpg'}" />
        <image :style="{width:50, height:50}" :source="require('../assets/favicon.png')" />
        <image :style="{width:200, height:150, marginTop:50}" :source="require('../assets/lake.webp')" />
    </view>
</template>

<style>
.container {
    margin: 5px;
}
.image {
    width: 100%;
    height: 200px;
    margin-bottom: 10px;
    border-radius: 15px;
}
</style>