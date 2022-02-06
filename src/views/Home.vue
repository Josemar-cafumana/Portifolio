<template>
 <main class="main">
    <div class="inicio">
        <div class="content">
          <div class="text mb-5"> 
              <h3>Olá, eu sou</h3>
              <h1>Josemar Cafumana</h1>
              <h3>Desenvolvedor Fullstack</h3>
          </div>
        <div class="botoes my-4">
              <a href="#" class="btn-gradient-purple me-4"><img src="../assets/linkedin.svg"> Linkedin</a>
              <a href="#"  class="btn-gradient-pink"> <img src="../assets/github.svg"> Github</a>
          </div>
        </div>
    </div>
    <section class="sobre-mim">
        <div class="dados-pessoais">
          <div class="row">
            <div class="image col-md-6 d-flex justify-content-center align-items-center mb-4">
              <div >

              </div>
            </div>
            <div class=" sobre col-md-6">
            
            <h3>Sobre mim</h3>
            <div class="descricao mt-5">
              <h4 class="my-3">Luanda,Angola</h4>
              <p class="mb-3">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent id egestas dui. Nullam finibus aliquam enim quis faucibus. Aenean ac commodo dolor, nec bibendum velit.</p>
            </div>
            <div class="redes-sociais">

           
            <div class="botoes">
                <a href="#" class="btn-gradient-purple me-4"><img src="../assets/linkedin.svg"> Currículo</a>
              <a href="#"  class="btn-gradient-pink"> <img src="../assets/github.svg"> E-mail</a>
            </div>
          </div>
            </div>
          </div>
          
         
        </div>
    </section>
 </main>
</template>

<script>
export default {
  name: "Home",
  components: {},
};
</script>
<style lang="scss">
    .inicio{
          width: 100%;
          height: 90vh;
          background:  url('../assets/Background-inicio.png') no-repeat;
          background-size: cover;
          background-position: center;
          position: relative;

          .content{
            
              position: absolute;
              left:10%;
              top:50%;
              transform: translate(-10%,-50%);

              .text{
                h1{
                  font-size: var(--font-size-1);
                  color: var(--primary);
                  font-weight: 600;
                  margin: 1rem 0;
                  line-height: 77px;
                  text-transform: uppercase;
                }
                h3{
                  text-transform: uppercase;
                  font-weight: 600;
                  font-size: var(--font-size-3);
                  color: var(--white);
                  line-height: 29px;
                }
              }
              .botoes{
              
           
              }
          }
             }

             .dados-pessoais{
                  .image div{
                    background: var(--dark);
                    width: 30rem;
                    height: 30rem;
                    object-fit: cover;
                    border-left: .2rem solid var(--primary);
                  }

                  .sobre{
                      h3{
                         text-transform: uppercase;
                  font-weight: 600;
                  font-size: var(--font-size-3);
                  color: var(--white);
                  line-height: 29px;
                      }
                      .descricao {
                        h4{
                          font-size: var(--font-size-4);
                          color: var(--white);
                        }
                        p{
                          font-size: var(--font-size);
                          color: var(--white);
                          max-width: 50rem;
                          margin-bottom: 2rem !important;
                        }
                      }
                  }
             }
</style>