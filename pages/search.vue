<template>
    <div>
        <div class="search">
        <b-container fluid>
            <b-row class="justify-content-center align-items-center">
                <b-col cols="12" md="8"> 
                    <b-row>
                        <b-col cols="12">
                            <nuxt-link to="/">
                                <img class="back-image" src="@/assets/img/search/left.svg" alt="Back Link">
                            </nuxt-link>    
                        </b-col>
                        <b-col cols="12" class="mt-4">
                            <h1 class="mb-0">Search Results</h1>
                            <h3>Open Data Challenge 2020</h3>
                        </b-col>
                        <b-col cols="12" class="mt-4" v-for="i of 6" :key="i">
                            <nuxt-link :to="`/organization/${i}`" class="search-results">
                                <h4 class="search-results__title">
                                    Open Data Challenge 2020
                                </h4>
                                <p class="search-results__description">
                                    Study after study proves diverse teams are more successful. Not only that, but teams that represent our population - and our customers
                                </p>
                            </nuxt-link>
                        </b-col>
                        <b-col cols="12" class="my-4">
                            <b-pagination
                                v-model="currentPage"
                                :total-rows="rows"
                                :per-page="perPage"
                                first-number
                            ></b-pagination>
                        </b-col>
                    </b-row>
                </b-col>
                <b-col cols="12" md="4">
                    <div class="filter d-flex flex-column align-items-start">
                        <h4>Filter</h4>
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