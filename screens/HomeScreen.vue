<template>
    <view>
        <text>
            Hola Mundo Home
        </text>

        <button title="Ir a Detalle" @press="goToDetail">

        </button>

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
        goToDetail(){
            this.navigation.navigate("Details")
        }
    },
}
</script>