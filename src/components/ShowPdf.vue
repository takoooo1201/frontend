<template>
    <div>
      <embed :src="pdfUrl" width="100%" height="600px" type="application/pdf" />
    </div>
  </template>
  
  <script>
const BaseURL = 'https://taipei-microservices-initiative-hayu.onrender.com/api/';
// const BaseURL = 'http://localhost:8081/api/';
  export default {

    data() {
      return {
        // /showpdf?file=filename
        pdfUrl: BaseURL + 'autofillform/showpdf/' + this.$route.query.file,
      };
    },
  };
  </script>