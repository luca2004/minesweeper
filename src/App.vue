<template>
  <v-app>
    <v-main>   
      <v-row>        
        <v-col cols="8">
          <grid />
          <timer />
        </v-col>
        <v-col cols="4"><HelpBlock /></v-col>
      </v-row>   
      
      
    </v-main>
  </v-app>
</template>

<script>
import Grid from "./components/Grid";
import Timer from "./components/Timer";
import HelpBlock from "./components/HelpBlock";
//import GitHub from "./components/GitHub";

export default {
  name: "App",

  components: {
    Grid,
    Timer,
    HelpBlock
    //GitHub
  },

  data: () => ({
    //
  })
};
</script>
<style>
#app {
  background: #bbb;
}
</style>

/**
app background
card theme
on hover card
 */