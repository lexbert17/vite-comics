<script>
import AppHeader from "./components/appHeader.vue"
import AppContent from "./components/AppContent.vue";
import AppNavigation from "./components/AppNavigation.vue"


export default {
  components: {
    AppHeader,
    AppContent,
    AppNavigation
},
}
</script>

<template>

<AppHeader/>
<AppContent/>
<AppNavigation/>
</template>

<style lang="scss">
@use "./style/general.scss";
*{
  margin: 0;
  box-sizing: border-box;
  padding: 0;
}
</style>
