<template>
    <div>
      <canvas ref="qrcodeCanvas"></canvas>
    </div>
  </template>
  
  <script>
  import QRCode from 'qrcode';
  
  export default {
    props: {
      link: {
        type: String,
        required: true,
      },
    },
    mounted() {
      this.generateQrCode(this.link);
    },
    methods: {
      async generateQrCode(link) {
        try {
          const canvas = this.$refs.qrcodeCanvas;
          await QRCode.toCanvas(canvas, link, {
            width: 300,
          });
        } catch (error) {
          console.error('Error generating QR code:', error);
        }
      },
    },
  };
  </script>
  