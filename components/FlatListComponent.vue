<template>
    <view>
        <flat-list 
            :style="{ height:300, backgroundColor:'red', padding:10}"
            :ListHeaderComponent="headerList()"
            :ListFooterComponent="footerList()"

            :data="[
                {
                    name: 'Andres'
                },
                {
                    name: 'Pepe'
                },
                {
                    name: 'Juan'
                },
                {
                    name: 'Manolo'
                },
                {
                    name: 'Ana'
                },
                {
                    name: 'Andres'
                },
                {
                    name: 'Pepe'
                },
                {
                    name: 'Juan'
                },
                {
                    name: 'Manolo'
                },
                {
                    name: 'Ana'
                },
            ]"
            :render-item="(item) => renderList(item)"
        />
    </view>
</template>

<script>

import React from 'react'

import { Text, View, Button } from 'react-native'

//import "" from './ItemListComponent.vue'

import ItemList from "./ItemListComponent.vue"

export default {
    methods: {
        headerList: function(){
            return <Button title="Botón arriba"></Button>
        },
        footerList: function(){
            return <View sytle={{height:10, width:"100%",backgroundColor: "#000", }} />
        },
        renderList: function(item){
            console.log(item)
            return <ItemList style={{ width: 100, height:300 }} title={item.item.name} />
            //return <Text style={{ height:100, width: 100 }}>{item.item.name}</Text>
        }
    },
}
</script>

<style>
.card {
    background-color:#FFFF00
}
</style>