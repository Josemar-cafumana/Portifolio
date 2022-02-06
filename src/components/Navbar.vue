<template>
  <header class="header px-5 ">
      <nav class="navbar navbar-expand-lg ">
  <div class=" container py-3 ">
    <a class="navbar-brand" href="/">Portfólio</a>
 

    <div @click="toggleMenu()" :class=" !navbar ? 'menu navbar-toggler' : ' menu navbar-toggler close '  " type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="line-1"></span>
        <span class="line-2"></span>
        <span class="line-3"></span>

    </div>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">

      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link "  href="/">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/about">Sobre mim</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/about">Experiência</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/about">Projectos</a>
        </li>
       
      </ul>
   
    </div>
  </div>
</nav>
  </header>
</template>

<script>
export default {
    name:"Navbar",
    data(){
        return {
            navbar: false
        }
    },
    methods: {
            toggleMenu(){
                    this.navbar = !this.navbar
            }
    }
}
</script>

<style lang="scss">

header{
    background: var(--dark);
}

.navbar{
    .menu {
        width: 3rem !important;
        height: 3rem !important;
      
        position: relative !important;
    
    &.close{
        height: 2rem;
        .line-1{
             transform: translate(-50%,-1px) rotate(-45deg);
        }
        .line-2{
            width: 0;
             transform: translate(-50%,4px);
        }
        .line-3{
             transform: translate(-50%,-1px) rotate(45deg);
        }

    }

        span{
            width: 100%;
            height: .15rem;
            background: var(--white);
            display: block !important;
         
            position: absolute;
            top:50%;left:50%;
            transform: translate(-50%,-50%);
        }

        .line-1{
             transform: translate(-50%,-10px) ;
        }
        .line-3{
             transform: translate(-50%,-3px) ;
        }
        .line-2{
            
             transform: translate(-50%,4px);
        }
    
    }
    .container{
            border-bottom: .20rem solid  var(--dark-200);
    }

    .navbar-brand{
        font-size: var(--font-size-3);
        color: var(--primary);
    }

    .navbar-nav .nav-link{
        color: var(--gray-light);
        font-size: var(--font-size);
        font-weight: 400;
        margin-left: 5rem;

        &:hover{
            color: var(--primary);
        }
    }
}
</style>