<template>
    <view>
        <text>
            Hola Mundo Detalle
        </text>

               <button title="Ir a Home" @press="goToHome"></button>
               <button title="Back" @press="goBack()"></button>

        
    </view>
</template>
<script>
export default {
    props: {
        navigation: {
            Object
        }
    },
    methods: {
        goToHome(){
            this.navigation.navigate("Home")
        },
        goBack(){
            this.navigation.goBack()
        }
    },
}
</script>