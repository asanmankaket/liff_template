<template>
    <div style="overflow: hidden;">
        <v-app-bar  dense flat >
            <v-toolbar-title class="pa-0">Contact Us</v-toolbar-title>
            
        </v-app-bar>
        
               <v-main >

            <div :style="{visibility: overlay ? 'hidden' : 'visible'}">

                <v-container  class="pt-10 pb-5 pr-0 pl-0"  >
                    <v-row>
                        <v-col cols="12" class="pl-10 pr-10">
                            
                                                
                            <div class="pb-0 blue--text  text-center  text-title font-weight-black">Computer Science</div>
                            <div class="pt-0 orange--text text-center   text-subtitle-2 font-weight-black">Faculty of Science and Technology</div>
                            
                            <div class="pb-10 pt-10  text-center blue--text">
                                <v-avatar
                                    color="white"
                                    rounded
                                    size="115"
                                    tile
                                    class="white--text"
                                    >
                                    
                                    <img
                                        src="https://sci.skru.ac.th/science/download/formdownload/logo/SciLogoPNG.png"
                                        alt="Sci - SKRU"
                                    >
                                </v-avatar>
                            </div>
                            <p>
                                <ul class="black--text lighten-2 text-body-2">
                                    <li>Computer Science, Faculty of Science and Technology</li>
                                    <li>email: comsci@skru.ac.th</li>
                                    <li>Tel: 074-999999</li>
                                    <li>Web: http://cs.skru.ac.th</li>
                                
                                </ul>

                            </p>
                                                    
                                                  


                        </v-col>
         
                    
                    </v-row>
                    <v-row  justify="center" >
                        <v-col
                            cols="12"
                            xs="12"
                            sm="6"
                            md="4"
                            lg="3"
                            xl="2"
                        >
                            <v-container class="pt-0 pb-0 pr-10 pl-10 text-center" v-if="showฺBack">
                                <v-btn rounded class="w-100  blue white--text">Back to Products</v-btn>
                            </v-container>

                        </v-col>
                    </v-row>
                    <v-row  justify="center" >
                        <v-col
                            cols="12"
                            xs="12"
                            sm="6"
                            md="4"
                            lg="3"
                            xl="2"
                        >
                            <v-container class="pt-0 pb-0 pr-10 pl-10 text-center">
                                <v-btn rounded class="w-100  main-btn" @click="close">Close</v-btn>
                            </v-container>

                        </v-col>
                    </v-row>
                </v-container> 



            </div>
            <v-overlay
            :opacity="1"
            :value="overlay"
            >
                <v-progress-circular indeterminate size="64">
                    Loading
                </v-progress-circular>
            </v-overlay>



        </v-main>

    </div>
</template>

<script>

export default {
    data() {
        return {

            //Variable Declaration

            overlay:true,

            
        }
    },
    async  mounted () {

         //Code 

        this.overlay=false
 

        
    },

    methods: {
        
        
        //Methods

    },

};
</script>

<style>
.v-tabs-slider-wrapper,  .v-tab--active {
  color: black !important;
  font-weight:bolder;

}

</style>