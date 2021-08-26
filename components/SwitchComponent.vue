<template>
    <view>
        <switch 
            :value="value"
            :on-change="onChange"
            :onValueChange="onValueChange"
            thumbColor="red"
            trackColor="yellow"
            :disabled="false"
        />
    </view>
</template>

<script>
export default {
    data() {
        return {
            value:false
        }
    },
    methods: {
        onChange: function(event){
            //console.log(event)
        },
        onValueChange: function(val){
            console.log(val)
            this.value = val
        }
    },
}
</script>