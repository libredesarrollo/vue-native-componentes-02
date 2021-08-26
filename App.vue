<template>
  <app-navigator></app-navigator>
</template>

<script>
import {
  createAppContainer,
  createStackNavigator,
} from "vue-native-router";

import HomeScreen from "./screens/HomeScreen.vue";
import DetailsScreen from "./screens/DetailsScreen.vue";
import ViewComponent from "./components/ViewComponent.vue";
import TextComponent from "./components/TextComponent.vue";
import TextInputComponent from "./components/TextInputComponent.vue";
import ButtonComponent from "./components/ButtonComponent.vue";
import ImageComponent from "./components/ImageComponent.vue";
import AlertComponent from "./components/AlertComponent.vue";
import ScrollViewComponent from "./components/ScrollViewComponent.vue";
import FlatListComponent from "./components/FlatListComponent.vue";
import ActivityIndicatorComponent from "./components/ActivityIndicatorComponent.vue";
import StatusBarComponent from "./components/StatusBarComponent.vue";
import SwitchComponent from "./components/SwitchComponent.vue";
import TouchableOpacityComponent from "./components/TouchableOpacityComponent.vue";

const StackNavigator = createStackNavigator(
  {
    Home: HomeScreen,
    Details: DetailsScreen,
    Views: ViewComponent,
    Text: TextComponent,
    TextInput: TextInputComponent,
    Button: ButtonComponent,
    Image: ImageComponent,
    Alert: AlertComponent,
    ScrollView: ScrollViewComponent,
    FlatList: FlatListComponent,
    ActivityIndicator: ActivityIndicatorComponent,
    StatusBar: StatusBarComponent,
    Switch: SwitchComponent,
    TouchableOpacity: TouchableOpacityComponent,
  },
  {
    initialRouteName: 'TouchableOpacity',
  }
);

const AppNavigator = createAppContainer(StackNavigator);

export default {
  components: { AppNavigator },
}
</script>