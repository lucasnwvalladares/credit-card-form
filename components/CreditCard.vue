<template>
    <div id="main">
        <div id="card-div" class="col-sm-12 col-lg-4">
            <div id="card-front" class="credit-card">
                <v-col id="card-front-content" cols="12">
                    <v-row id="front-up">
                        <div id="big-ball"></div>
                        <div id="small-ball"></div>
                    </v-row>
                    <v-row>
                        <v-col>
                            <div id="front-botton">
                                <v-row>
                                    <h2>0000 0000 0000 0000</h2>
                                </v-row>
                                <v-row>
                                    <v-col class="credentials">
                                        <p id="name-cred">JOHN DOE</p>
                                    </v-col>
                                    <v-col class="credentials">
                                        <p id="valid-cred">MM/YY</p>
                                    </v-col>
                                </v-row>
                            </div>
                        </v-col>
                    </v-row>
                </v-col>
            </div>
            <div id="card-back" class="credit-card">
                <div class="card-back-row"></div>
                <div class="card-back-row">
                    <div id="cvc-place">
                        <p>123</p>
                    </div>
                </div>
                <div class="card-back-row"></div>
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
        font-family: 'Space Grotesk', sans-serif;
        font-size: 18px;
    }

    .credit-card {
        height: 200px;
        width: 400px;
        margin-top: 30px;
        border-radius: 4%;
    }

    #card-front {
        background: hsl(279, 6%, 55%);
        padding: 2rem;
    }

    #card-front-content {
        display: flex;
        flex-direction: column;
        row-gap: 40px;
    }

    .credentials {
        display: flex;
        flex-direction: row;
        font-size: 15px;
        padding: 0;
        margin-top: 10px;
    }

    .credentials:last-of-type {
        justify-content: flex-end;
    }

    #big-ball {
        --size: 40px;
        background: white;
        border-radius: 50%;
        width: var(--size);
        height: var(--size);
    }

    #small-ball {
        --size: 20px;
        background: inherit;
        border-radius: 50%;
        width: var(--size);
        height: var(--size);
        border: 1px solid white;
        margin-top: 10px;
        margin-left: 10px;
    }

    #card-back {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        background: hsl(270, 3%, 87%);
    }

    .card-back-row {
        height: 50px;
    }

    .card-back-row:first-of-type {
        background: rgb(27, 27, 27);
        margin-top: 10px;
    }

    .card-back-row:nth-of-type(2) {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    #cvc-place {
        background: #acadb3;
        height: 80%;
        width: 80%;
        border-radius: 5%;
    }

    #cvc-place:first-child {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        padding-right: 20px;
        color: white;
    }

    #form-div {
        background: pink;
        position: relative;
        display: block;
        margin-left: 66,6%;
    }
</style>