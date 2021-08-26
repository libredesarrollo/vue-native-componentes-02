<template>
    <view class="container">
        <button color="green" :title="boton" @press="myClick">

        </button>
    </view>
</template>

<script>
export default {
    data() {
        return {
            boton:"My Botón"
        }
    },
    methods: {
        myClick() {
            //alert("Hola Mundo")
            this.boton = "Click en el botón"
        }
    },
}
</script>

<style>
.container {
    margin: 5px;
}

</style>