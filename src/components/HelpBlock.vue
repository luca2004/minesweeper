<template>
  <v-container>
    <v-row justify="center" align="center" class="ma-8">
      <p class="mb-0">Help</p>
      <p class="ml-2 mb-0">{{ nbHelp }}</p>
      <v-spacer></v-spacer>
      <v-btn icon @click="help_click()"><v-icon>mdi-account-question</v-icon></v-btn>
    </v-row>
    
  </v-container>
</template>

<script>
import { mapActions, mapGetters } from "vuex";
export default {
    name: "HelpBlock",
    components: {  },   
    computed: {
        ...mapGetters({
            nbHelp: "grid/getHelps",     
        })
    }, 
    methods: {
        ...mapActions("grid", ["help4Flag"]),
        help_click(){
            this.help4Flag();
        }
    }
}
</script>