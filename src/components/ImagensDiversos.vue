<template>
   <div class="containerImagem">
    
    <img v-lazy="imageSrc" 
    alt="imagem 1" class="ImagemUnicaAltura400px">
    </div>
    <div class="divImagemMeiaTela">
        <img src="@/assets/cafethe.jpg" alt="imagem 2">
        <img src="@/assets/cafemaq.jpg" alt="imagem 3">  
      </div>
     
      <picture>
  <source srcset="image.webp" type="image/webp">
  <img src="image1.jpg" alt="Descrição da imagem">
</picture>

    </template>
    
    <script> 
     import {ref} from 'vue';
const imageSrc = ref ("@/assets/cafegosto.jpg");
    export default {
        name: 'ImagensDiversos',
        props: {
            msg: String, imageSrc 
        }
    }
    </script>
    
    <!--Add "scoped" atribute to limite css to this component only-->
    <style scoped></style>