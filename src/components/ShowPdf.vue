<template>
    <div>
        <h1>Click to Download</h1>
        <h3>{{ this.BaseURL + 'autofillform/showpdf/' + this.$route.query.file  }}</h3>
    </div>
    <div>
        <QrCode :link="this.BaseURL + 'autofillform/showpdf/' + this.$route.query.file" />
    </div>
</template>

<script>
import QrCode from './QRcode.vue';
export default {
    components: {
        QrCode,
    },
    data() {
        return {
            BaseURL: 'https://taipei-microservices-initiative-hayu.onrender.com/api/',
            link: this.BaseURL + 'autofillform/showpdf/' + this.$route.query.file,
        };
    },
    mounted() {
        console.log(this.BaseURL);
    }
};
</script>


<style scoped>
canvas {
    border: 1px solid black;
}
</style>