<template>
    <div style="overflow: hidden;">
        <v-app-bar  dense flat >
            <v-toolbar-title class="pa-0">Products</v-toolbar-title>
            <v-btn 
                icon
                color="white"
                
            >
                <v-icon>mdi-card-account-mail</v-icon>
            
            </v-btn>
        </v-app-bar>
        
               <v-main >

            <div :style="{visibility: overlay ? 'hidden' : 'visible'}">

                <v-container  class="pt-3 pb-5 pr-0 pl-0"  >
                    <v-row>
                        <v-col cols="12" class="pl-10 pr-10">
                            <v-tabs
                                class="pb-5"
                                v-model="tab"
                                centered
                                slider-color="black"
                                
                            >

                                <v-tab
                                    href="#basic"
                                >
                                    BASIC
                                </v-tab>


                                <v-tab
                                    href="#pro"
                                >
                                    PRO
                                </v-tab>

                                <v-tab
                                    href="#business"
                                >
                                    BUSINESS
                                </v-tab>

                
                                
                            </v-tabs>

                            <v-tabs-items v-model="tab">
                                <v-tab-item
                                    value="basic"
                                >
                                     <v-container fluid>
                                        <v-row dense justify="center">
                                            <v-col
                                               
                                                cols="12"
                                                xs="12"
                                                sm="12"
                                                md="12"
                                                lg="10"
                                                xl="8"
               
                                            >

                                                
                                                <v-card
                                                    class="mb-5 pt-0 pb-0 pl-0 pr-0 rounded-lg "
                                                    outlined elevation="3"
                                                >

                                                    <v-card-text>
                                                    <div class="pb-1 black--text text-subtitle-1 font-weight-black">Personal meetings</div>
                                                    <div class="pb-10 pt-10 text-h4  text-center blue--text">
                                                        Free
                                                    </div>
                                                    <p>
                                                        <ul class="black--text lighten-2 text-body-2">
                                                          
                                                            <li>Host up to 100 participants</li>
                                                            <li>Unlimited group meetings for up to 40 minutes</li>
                                                            <li>Unlimited one-to-one meetings with a 30 hour time limit per meeting.</li>
                                                            <li>Private & Group Chat</li>
                                                        </ul>

                                                    </p>
                                                    
                                                    </v-card-text>
                                                    <v-card-actions class='pb-5'>
                                                    
                                                        <v-btn
                                                            small
                                                            rounded
                                                            class="w-100  font-weight-regular white--text "
                                                            color="blue darken-3"
                                                            
                                                          
                                                        >
                                                            Select this package
                                                        </v-btn> 

                                                    </v-card-actions>

                                                   
                                                </v-card>





                                            </v-col>
                                        </v-row>
                                     </v-container>
                                     

                                   

  
                                </v-tab-item>
                                <v-tab-item
                                    value="pro"
                                >


                                    <v-container fluid>
                                        <v-row dense>
                                            <v-col
                                      
                                                cols="12"
                                                xs="12"
                                                sm="12"
                                                md="12"
                                                lg="10"
                                                xl="8"
                                            >

                                                <v-card
                                                    class="mb-5 pt-0 pb-0 pl-0 pr-0 rounded-lg "
                                                    outlined elevation="3"
                                                >

                                                    <v-card-text>
                                                    <div class="pb-1 black--text text-subtitle-1 font-weight-black">Great for small teams</div>
                                                    <div class="pb-0 pt-10 text-h4  text-center blue--text">
                                                        $149.90
                                                    </div>
                                                    <div class="pb-10 grey--text text-center text-subtitle-2 ">1 license/1 year</div>
                                                    <p>
                                                        <ul class="black--text lighten-2 text-body-2">
                                                          
                                                            <li>Host up to 100 participants</li>
                                                            <li>Increase participants up to 1,000 with Large Meetings add-on</li>
                                                            <li>Group meetings for up to 30 hours</li>
                                                            <li>Social media streaming</li>
                                                            <li>1 GB cloud recording (per license)</li>
                                                        </ul>

                                                    </p>
                                                    
                                                    </v-card-text>
                                                    <v-card-actions class='pb-5'>
                                                            
                                                                <v-btn
                                                                    small
                                                                    rounded
                                                                    class="w-100  font-weight-regular white--text "
                                                                    color="blue darken-3"
                                                                    
                                                                   
                                                                >
                                                                    Select this package
                                                                </v-btn> 
                                                       
                                                               


                                                    </v-card-actions>

                                                   
                                                </v-card>

                                            </v-col>
                                        </v-row>
                                     </v-container>


                                  
                                </v-tab-item>
                                <v-tab-item
                                    value="business"
                                >


                                    <v-container fluid>
                                        <v-row dense>
                                            <v-col
                                      
                                                cols="12"
                                                xs="12"
                                                sm="12"
                                                md="12"
                                                lg="10"
                                                xl="8"
                                            >

                                                <v-card
                                                    class="mb-5 pt-0 pb-0 pl-0 pr-0 rounded-lg "
                                                    outlined elevation="3"
                                                >

                                                    <v-card-text>
                                                    <div class="pb-1 black--text text-subtitle-1 font-weight-black">Small businesses</div>
                                                    <div class="pb-0 pt-10 text-h4  text-center blue--text">
                                                        $199.90
                                                    </div>
                                                    <div class="pb-10 grey--text text-center text-subtitle-2 ">1 license/1 year</div>
                                                    <p>
                                                        <ul class="black--text lighten-2 text-body-2">
                                                          
                                                            <li>Host up to 300 participants</li>
                                                            <li>Increase participants up to 1,000 with Large Meetings add-on</li>
                                                            <li>Single sign-on</li>
                                                            <li>Recording transcripts</li>
                                                            <li>Managed domains</li>
                                                            <li>Company branding</li>
                                                            <li>Up to 99 licenses</li>
                                                        </ul>

                                                    </p>
                                                    
                                                    </v-card-text>
                                                    <v-card-actions class='pb-5'>
                                                            
                                                                <v-btn
                                                                    small
                                                                    rounded
                                                                    class="w-100  font-weight-regular white--text "
                                                                    color="blue darken-3"
                            
                                                                >
                                                                    Select this package
                                                                </v-btn> 
                                                       
                                                               


                                                    </v-card-actions>

                                                   
                                                </v-card>

                                            </v-col>
                                        </v-row>
                                     </v-container>


                                  
                                </v-tab-item>
                            
                            
                            </v-tabs-items>



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
                                <v-btn rounded class="w-100  main-btn" @click = "Close">Close</v-btn>
                            </v-container>

                        </v-col>
                    </v-row>
                </v-container> 
                <v-snackbar
                    v-model="snackbar"
                    >
                    {{ text }}

                    
                </v-snackbar>


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
            webhook:process.env.WEBHOOK_API_URI,
            tab:'basic',
            
            overlay:true,
            snackbar: false,
            text: `Package Selected!`,
          
            
        }
    },
    async  mounted () {

        //Code 


        this.overlay=false

    },

    methods: {
        close(){
            liff.closeWindow()
        }
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