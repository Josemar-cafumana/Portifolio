<template>
 <main class="main">
    <div class="inicio">
        <div class="content ">
          <div class="text mb-5"> 
              <h3>Olá, eu sou</h3>
              <h1>Josemar Cafumana</h1>
              <h3>Desenvolvedor Full-stack</h3>
          </div>
        <div class="botoes my-4">
              <a href="#" class="btn-gradient-purple me-4"><img alt="logo do linkedin" src="../assets/linkedin.svg"> Linkedin</a>
              <a href="#"  class="btn-gradient-pink"> <img  alt="logo do github" src="../assets/github.svg"> Github</a>
          </div>
        </div>
    </div>
    <!-- Seção sobre mim -->
    <section class="sobre-mim">
        <div class="dados-pessoais">
          <div class="row">
            <div class="image col-md-6 d-flex justify-content-center align-items-center mb-4">
              <div class="image-wrapper" >
                 <img src="../assets/josemar.jpg" alt="foto pessoal">
              </div>
            </div>
            <div class=" sobre col-md-6 d-flex justify-content-start align-items-center ">
            
            <div class="sobre-wrapper">
            <h3>Sobre mim</h3>
            <div class="descricao mt-5">
              <h4 class="my-3">Luanda, Angola</h4>
              <p class="mb-3">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent id egestas dui. Nullam finibus aliquam enim quis faucibus. Aenean ac commodo dolor, nec bibendum velit.</p>
            </div>
            <div class="redes-sociais ">
                <a href="#"><img alt="logo do twitter" src="../assets/twitter.svg"></a>
                <a href="#"><img  alt="logo do twitch" src="../assets/twitch.svg"></a>
                <a href="#"><img  alt="logo do youtube" src="../assets/youtube.svg"></a>
                <a href="#"><img  alt="logo do figma" src="../assets/figma.svg"></a>
                <a href="#"><img  alt="logo do codepen" src="../assets/codepen.svg"></a>
                <a href="#"><img  alt="logo do facebook" src="../assets/facebook.svg"></a>
            </div>
            <div class="botoes my-3">
                <a href="#" class="btn-gradient-purple me-4"><img alt="icone download" src="../assets/download-cloud.svg"> Currículo</a>
              <a href="#"  class="btn-gradient-pink"> <img  alt="icone email" src="../assets/mail.svg"> E-mail</a>
            </div>

            </div>
        
         
            </div>
          </div>
          
         
        </div>
    </section>

    <section class="experiencia px-5">
      <h3>Experiência</h3>
        <div class="row d-flex justify-content-center">
          <div class="menu-experiencia col-md-4  ">
              <ul class="list-unstyled">
                <li>Freelancer</li>
                <li>Código Fonte TV</li>
                <li>Zuplae</li>
                <li>ContWeb</li>
                <li>iuricode</li>
                <li>Digital House</li>
              </ul>
          </div>
          <div class="experiencia-info col-md-7 ">
                  <div class="content w-100">
                    <div class="experiencia-info-header d-flex justify-content-between align-items-center mb-3   mb-5">
                      <h3 >Professor conteudista em Frontend</h3>
                      <p >Nov 2021 - Atual</p>
                    </div>
                    <div class="experiencia-info-descricao">
                      <h6>Digital House</h6>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque eu purus risus. Ut rutrum sollicitudin purus in accumsan. Proin at mattis metus. Nullam sit amet mauris condimentum, volutpat augue in, mattis urna.
                      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque eu purus risus. Ut rutrum sollicitudin purus in accumsan.</p>
                    </div>
                  </div>
          </div>
        </div>
    </section>

    <section class="projectos">
      <h3>Projectos</h3>
      
      <div class="row ">

        <div  class=" box-image col-md-6  d-flex justify-content-center align-items-center my-5" v-for="projecto in projectos" :key="projecto.id">
           <Projectos :projectos="projecto" />
        </div>
      
      </div>
    </section>

 </main>
</template>

<script>
import Projectos from '@/components/Projectos.vue'

export default {
  name: "Home",
  data(){
    return {
          projectos: [
            {id:1, titulo: "Website de Construção"},
            {id:2, titulo: 'Restaurante Website'},
            {id:3, titulo: "Website de Construção"},
            {id:4, titulo: 'Restaurante Website'},
          ]
    }
  },
  components: {
    Projectos
  },
};
</script>
<style src="./Home.scss" lang="scss"></style>