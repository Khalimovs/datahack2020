<template>
    <div class="reference">
        <section class="section">
            <b-container fluid>
                <b-row>
                    <b-col cols="12">
                        <h4>References</h4>
                    </b-col>
                    <b-col cols="12" v-for="i of links" :key="i.id">
                        <p>
                            <nuxt-link to="/">
                                {{ i.title }}
                            </nuxt-link>
                        </p>
                    </b-col>
                </b-row>
            </b-container>
        </section>
    </div>
</template>

<script>
export default {
    data() {
        return {
            links: [
                { id: 1, title: 'Prices for KIA cars in Uzbekistan published' },
                { id: 2, title: 'WB approves funding for construction of a solar power plant in Navoi region' },
                { id: 3, title: 'Uzbekistan increases import of foreign-made cars in Jan-Aug' },
                { id: 4, title: 'Volswagen Uzbekistan sells 100 Caddy cars in over a month' },
                { id: 5, title: 'New Skoda crossover to enter Uzbek market in October' },
            ]
        }
    }
}
</script>