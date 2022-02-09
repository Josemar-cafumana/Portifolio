<template>
         <div class="box">
              <div class="image">
                 <!-- <img :src="projectos.image  " alt=""> -->
              </div>
              <div class="descricao">
                  <h3>{{ projectos.titulo }}</h3>
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus blandit interdum odio eu varius.</p>
              </div>
              <div class="tecnologias">
                   <img src="../assets/html.svg" alt="html">
                  <img src="../assets/css.svg" alt="css">
                  <img src="../assets/javascript.svg" alt="javascript">
              </div>
              <a href="#" class="btn-gradient-purple mt-5"> <img src="../assets/link.svg">Visualizar</a>
            </div>
</template>

<script>
export default {
        name: "Projectos",
        props:{
            projectos: Array
        }
}
</script>

