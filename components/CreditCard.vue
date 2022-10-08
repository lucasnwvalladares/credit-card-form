<template>
    <div id="main">
        <div id="card-div" class="col-sm-12 col-lg-4">
            <div id="card-front" class="credit-card">
                <v-col cols="12">
                    <v-row>
                        <div id="front-top">
                            <div id="big-ball"></div>
                            <div id="small-ball"></div>
                        </div>
                    </v-row>
                    <v-row>
                        <div id="front-botton">
                            <v-row>
                                <h1>0000 0000 0000 0000</h1>
                            </v-row>
                            <v-row>
                                <v-col>
                                    JOHN DOE
                                </v-col>
                                <v-col>
                                    MM/YY
                                </v-col>
                            </v-row>
                        </div>
                    </v-row>
                </v-col>
            </div>
            <div id="card-back" class="credit-card">
                <v-col>
                    <v-row>
                        <div></div>
                    </v-row>
                    <v-row>
                        <div></div>
                    </v-row>
                    <v-row>
                        <div></div>
                    </v-row>
                </v-col>
            </div>
        </div>
        <div id="form-div" class="col-sm-12 col-lg-8">
            <div>
                <v-form>
                    <v-col cols="4">
                        <v-row>
                            <v-col cols="12">
                                <v-field>
                                    <v-label>CARDHOLDER NAME</v-label>
                                    <v-text-field placeholder="e.g. Jane Appleseed" solo dense></v-text-field>
                                </v-field>
                            </v-col>
                        </v-row>
                        <v-row>
                            <v-col cols="12">
                                <v-field>
                                    <v-label>CARD NUMBER</v-label>
                                    <v-text-field placeholder="e.g. 0000 0000 0000 0000" solo dense></v-text-field>
                                </v-field>
                            </v-col>
                        </v-row>
                        <v-row>
                            <v-col cols="6">
                                <v-field>
                                    <v-label>EPX. DATE (MM/YY)</v-label>
                                    <v-row>
                                        <v-col>
                                            <v-text-field placeholder="MM" solo dense></v-text-field>
                                        </v-col>
                                        <v-col>
                                            <v-text-field placeholder="YY" solo dense></v-text-field>
                                        </v-col>
                                    </v-row>
                                </v-field>
                            </v-col>
                            <v-col cols="6">
                                <v-field>
                                    <v-label>CVC</v-label>
                                    <v-text-field placeholder="e.g. 123" solo dense></v-text-field>
                                </v-field>
                            </v-col>
                        </v-row>
                        <v-row>
                            <v-col cols="12">
                                <v-btn>Confirm</v-btn>
                            </v-col>
                        </v-row>
                    </v-col>
                </v-form>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scope>
    #main {
        display: flex;
    }

    #card-div {
        
    }

    .credit-card {
        height: 150px;
        width: 300px;
        margin-top: 30px;
        border-radius: 4%;
    }

    #card-front {
        background: lightblue;
        padding: 2rem;
    }

    #card-back {
        background: green;
    }

    #form-div {
        background: pink;
        position: relative;
        display: block;
        margin-left: 66,6%;
    }
</style>