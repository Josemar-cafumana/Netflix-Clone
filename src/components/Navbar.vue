<template>
  <header >
    <b-navbar variant="faded" type="light" class="d-flex justify-content-between">
            <b-navbar-brand href="#">
            <img src="@/assets/logo.svg" class="logo" alt="Logo da netflix">
            </b-navbar-brand>

            <div class="button" >
                  <b-button variant="danger">Sign In</b-button>
            </div>
  </b-navbar>
  </header>
</template>

<script>
export default {
        name: 'Navbar'
}
</script>

<style lang="scss" scoped>

    header{
      position: absolute;
      top: 0;right: 0;left: 0;
      z-index: 999;
      padding: 0.5rem 3rem;
    }
    .logo{
      width: 8rem ;
    
    }
</style>