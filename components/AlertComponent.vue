<template>
  <view>
    <button @press="dameUnClick" title="Uso de alert"></button>
  </view>
</template>

<script>
import { Alert } from "react-native";

export default {
  methods: {
    dameUnClick() {
      //alert("Me diste un click!")

      Alert.alert("Titulo de la alerta", "Este es el contenido", [
        { text: "Si", onPress: () => console.log("Me diste un clic Si") },
        {
          text: "Cancelar",
          onPress: () => console.log("Me diste un clic cancelar"),
        },
        {
          text: "Otro!",
          onPress: () => {
            console.log("Me diste un en otro 1");
            console.log("Me diste un en otro 2");
          },
        },
      ]);
    },
  },
};
</script>