<template>
    <div class="card-wrapper pr-3">
        <div class="card-wrapper__header">
            <img :src="require( `@/assets/img/index/${item.id}.svg` )" :alt="item.title" :style="(item.id == 2 || item.id == 4) ? 'width: 76px;' : ''">
            <h2>{{ item.title }}</h2>
        </div>
        <div class="card-wrapper__description">
            <p>{{ item.description }}</p>
        </div>
    </div>
</template>

<script>
export default {
    props: ['item']
}
</script>