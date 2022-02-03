<template>
  <header :class="home ? 'home' : '' " >
    <b-navbar toggleable="lg" variant="faded" type="light" class="d-flex justify-content-between">
            <b-navbar-brand href="#">
            <img src="@/assets/logo.svg" class="logo" alt="Logo da netflix">
            </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav v-if="home">
      <b-navbar-nav class="text-white ml-4">
        <b-nav-item href="/home">Inicio</b-nav-item>
        <b-nav-item href="#">Series</b-nav-item>
        <b-nav-item href="#">Filmes</b-nav-item>
        <b-nav-item href="#">Mais Recentes</b-nav-item>
        <b-nav-item href="#">Minha Biblioteca</b-nav-item>
       
    
      </b-navbar-nav>
    </b-collapse>

 

            <div class="button" v-if="!home" >
                  <b-button variant="danger">Sign In</b-button>
            </div>
               <b-navbar-nav class="text-white ml-auto d-flex flex-row" v-if="home">
    
        <b-nav-item href="#"><b-icon icon="search"></b-icon></b-nav-item>
        <b-nav-item href="#"><b-icon icon="bell-fill"></b-icon></b-nav-item>
        <b-nav-item href="/"><img alt="perfil netflix" src="../assets/img/profile.jpg" ></b-nav-item>
    
      </b-navbar-nav>
  </b-navbar>
  </header>
</template>

<script>
export default {
        name: 'Navbar',
        props: {
          home: Boolean
        },
}
</script>

<style lang="scss" scoped>

    header{
      position: absolute;
      top: 0;right: 0;left: 0;
      z-index: 999;
      padding: 0.5rem 3rem;

      &.home{
        background: transparent;
        position:fixed !important;
      }
    }
    .logo{
      width: 8rem ;
    }
    .nav-link{
      color: white;
      font-size: var(--font-size) !important;
      padding: 0 .5rem;

      img{
        width: 2rem;
      }
      
    }
</style>