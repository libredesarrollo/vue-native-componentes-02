<template>
    <view>
        
        <touchable-opacity :on-press="MyClick">
            <text :style="{padding:10, backgroundColor:'red'}">
                Boton personalizado
            </text>
        </touchable-opacity>

    </view>
</template>

<script>
export default {
    methods: {
        MyClick: function(){
            alert("Hola Mundo")
        }
    },
}
</script>