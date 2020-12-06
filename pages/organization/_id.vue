<template>
    <div>
        <div class="detail">
        <b-container fluid>
            <b-row class="justify-content-center align-items-center">
                <b-col cols="12" md="8"> 
                    <b-row>
                        <b-col cols="12">
                            <nuxt-link to="/search">
                                <img class="back-image" src="@/assets/img/search/left.svg" alt="Back Link">
                            </nuxt-link>    
                        </b-col>
                        <b-col cols="12" class="mt-4">
                            <h1 class="mb-0">Open Data Challenge 2020 </h1>
                            <h3>Held by IT Park</h3>
                        </b-col>
                        <b-col cols="12" class="mt-4">
                            <h3 class="greeen my-4">Follow the data</h3>
                            <p>
                                 Study after study proves diverse teams are more successful. Not only that, but teams that represent our population - and our customers will have a greater impact.
                                 Like any business with big dreams, we measure what matters, set aggressive goals, and hold ourselves accountable. 
                                 Diversity, equity, and inclusion are certainly no exception. Study after study proves diverse teams are more successful. Not only that , but teams that 
                                 represent our population -  and our customers - will have a greater impact. Like any business with big dreams.
                            </p>
                            <h3 class="greeen my-4">Gallery</h3>
                            <div class="d-flex flex-row justify-content-between">
                                <img src="https://it-park.uz/storage/images/news/normal/gYJrOz9rQVbD9fs3QVb80lGiWQiLWYC4kSdqLYWv.jpeg" style="border-radius: 10px" alt="" height="140px" width="160px">
                                <img src="https://it-park.uz/storage/images/news/normal/gYJrOz9rQVbD9fs3QVb80lGiWQiLWYC4kSdqLYWv.jpeg" style="border-radius: 10px" alt="" height="140px" width="160px">
                                <img src="https://it-park.uz/storage/images/news/normal/gYJrOz9rQVbD9fs3QVb80lGiWQiLWYC4kSdqLYWv.jpeg" style="border-radius: 10px" alt="" height="140px" width="160px">
                                <img src="https://it-park.uz/storage/images/news/normal/gYJrOz9rQVbD9fs3QVb80lGiWQiLWYC4kSdqLYWv.jpeg" style="border-radius: 10px" alt="" height="140px" width="160px">
                            </div>
                            <nuxt-link to="/winner/3" style="text-decoration: none !important;">
                                <h3 class="greeen my-4">
                                    Winners
                                </h3>
                            </nuxt-link>
                            <div class="participators">
                                <p>1. Global Tech Team</p>
                                <p>2. Dolor sit </p>
                                <p>3. Amet</p>
                            </div>
                            <h3 class="greeen my-4">Other contestants</h3>
                            <div class="participators">
                                <p>1. DEI is a living</p>
                                <p>2. breathing thing</p>
                                <p>3. and just like</p>
                                <p>4. and great product</p>
                            </div>
                        </b-col>
                    </b-row>
                </b-col>
                <b-col cols="12" md="4">
                    <div class="filter">
                        <div class="d-flex flex-row justify-content-between align-items-center">
                            <h4>Investment need</h4>
                            <img src="@/assets/img/prize.svg" alt="" width="30px">
                        </div>
                        <h2>$50 000</h2>
                        <!-- <b-button class="contact mt-auto w-100">
                            Contact now 
                            <b-icon icon="arrow-right" class="ml-2"></b-icon>
                        </b-button> -->
                    </div>
                    <div class="filter mt-5">
                        <div class="d-flex flex-row justify-content-between align-items-center">
                            <h4>Notes</h4>
                            <img src="@/assets/img/pin.svg" alt="" width="30px">
                        </div>
                        <p class="my-3">While talent and potential are equally distributed, opportunity is not. While talent and potential
                            are equally distributed, opportunity is not. We recruit people from under represented group while talent.
                        </p>
                        <!-- <b-button class="contact mt-auto w-100">
                            Contact now 
                            <b-icon icon="arrow-right" class="ml-2"></b-icon>
                        </b-button> -->
                    </div>
                    <div class="filter mt-5">
                        <div class="d-flex flex-row justify-content-between align-items-center">
                            <h4>Get in touch</h4>
                            <img src="@/assets/img/contact.svg" alt="" width="30px">
                        </div>
                        <p class="my-3">
                            You can contact the competition mentors to find the contacts of contestans or get more of an information.
                        </p>
                        <p>
                            <b class="text-underline">Phone: (98) 765 43 21 </b>
                        </p>
                        <b-button class="contact mt-auto w-100">
                            Contact now 
                            <b-icon icon="arrow-right" class="ml-2"></b-icon>
                        </b-button>
                    </div>
                </b-col>
            </b-row>
        </b-container>
    </div>
    <Reference />
    </div>
</template>

<script>
import Reference from "@/components/Reference";

export default {
    components: {
        Reference,
    },
    data() {
        return {
            rows: 100,
            perPage: 1,
            currentPage: 5
        }
    }
}
</script>

