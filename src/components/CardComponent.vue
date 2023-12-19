<template>
        <div class="card">
          <img :src="image"  class="card-img-top" :alt="title">
          <div class="card-body">
            <h5  :headerClass="headerClass">{{ title }}</h5>
            <p class="card-text">{{ body }}</p>
            <a :href="link">{{ link }}</a>
          </div>
        </div>
</template>


<script  lang="ts">
export default {
    name: "CardComponent",
    props: {
        title: String,
        image: String,
        body: String,
        link: String,
        headerClass: String
    }
}

</script>

<style scoped lang="scss">
@import '../assets/css/_colorPalette.scss';

.card {
    width: 18rem;
    margin: 1rem;
}

.color-liberty-opacity {
    color: $color-aqua-marine;
}
</style>

