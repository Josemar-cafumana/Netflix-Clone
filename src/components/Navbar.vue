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

<style src="./style.scss" lang="scss" scoped></style>