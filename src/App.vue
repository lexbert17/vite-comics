<script>
import AppHeader from "./components/appHeader.vue"
import AppContent from "./components/AppContent.vue";
import AppNavigation from "./components/AppNavigation.vue"
import AppDcListVue from "./components/AppDcList.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppContent,
    AppNavigation,
    AppDcListVue,
    AppFooter
},
}
</script>

<template>

<AppHeader/>
<AppContent/>
<AppNavigation/>
<AppDcListVue/>
<AppFooter/>
</template>


<style lang="scss">
@use "./style/general.scss";

</style>
