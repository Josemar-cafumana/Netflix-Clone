<template>
  <div class="home">
      <Navbar :home="true" />
      <div class="banner px-4">
            <div class="escurecer"></div>

            <div class="content">
                    <h1>Money Heist</h1>
                    <div class="botoes my-4">
                        <a href="#"><b-icon icon="play-fill"></b-icon>Play</a>
                        <a href="#" class="ml-4"><b-icon icon="plus"></b-icon>My List</a>
                    </div>
                    <div class="descricao">
                        <h2>Watch part 3 Now</h2>
                        <p>With million of euros and their lives on the line, nine robbers attempt to pull off the greatest heist of all time.</p>
                    </div>
            </div>
      </div>
  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'

export default {
        name:'Home',
        components: {
            Navbar
        }
}
</script>

<style lang="scss">
.banner{
    height: 100vh;
    background: url('../assets/img/home-banner.jpg') no-repeat;
    background-size: cover;
    background-position: center;
    position: relative;

    .escurecer{
  
        width: 100%;
        height: 100%;
        background: rgba($color: #000000, $alpha: .3)
    }
    .content{
        position: absolute;
        left: 10%;
        top:50%;
        transform: translateY(-50%);


        h1{
            font-size: 6rem;
            font-weight: bold;
            margin: .5rem 0;
        }
        .botoes{

            a{
                background:  rgba($color: #e7e7e7, $alpha: .2);
                padding: .5rem 2rem;
                text-align: center;
                border-radius: .1rem;
                font-size: 1.5rem;
                font-weight: bolder;
                text-decoration: none;


                &:hover{
                    background: #000000;
                }

                svg{
                    margin-right: .3rem;
                    
                }
            }
        }
    }
}
</style>