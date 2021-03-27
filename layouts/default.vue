<template>
  <div>
    <TheHeader @sidenavToggle="displaySidenav = !displaySidenav" />
    <TheSideNav :show="displaySidenav" @close="displaySidenav = false" />

    <Nuxt />
  </div>
</template>

<style>
html {
  font-family: 'Open Sans', sans-serif;
}

body {
  margin: 0;
}
</style>

<script>
import TheHeader from '@/components/Navigation/TheHeader';
import TheSideNav from '@/components/Navigation/TheSidenav';

export default {
  data() {
    return {
      displaySidenav: false,
    };
  },
  components: {
    TheHeader,
    TheSideNav,
  },
};
</script>
