<template>
  <div class="accordion" id="accordionExample">
              <div class="card" v-for="card in cards" :key="card.id">
                <div class="card-header" id="headingOne">
                  <h2 class="mb-0">
                    <button class="btn btn-link btn-block text-left" type="button" data-toggle="collapse" :data-target="'#collapse'+card.id" aria-expanded="true" aria-controls="collapseOne">
                    {{ card.titulo }}
                    </button>
                  </h2>
                </div>

                <div :id="'collapse'+card.id" class="collapse" aria-labelledby="headingOne" data-parent="#accordionExample">
                  <div class="card-body">
                   {{ card.descricao }}
                  </div>
                </div>
              </div>
             
 
      </div>
</template>

<script>
export default {
    name: 'Card-faq',
    props: {
        cards: Array
    }

}
</script>

<style lang="scss" scoped>
.card{
    margin-bottom: .5rem;
    .card-header{
        padding: .8em 2.2em 0.8em 1.2em;
        background: #303030;
        

        .btn-link{
            font-size: var(--font-size-2) !important;
            color: var(--white);
            text-decoration: none !important;
      
       

            &::after{
                content: '\002b';
                position: absolute;
                width: 50px;
                font-size:2.5rem;
                right:0;
                top: 5px;
                color:white;
            }


          
        }
    }
    .card-body{
        background: #303030;
       border-top: .10rem solid #000 !important;
       font-size: var(--font-size);
    }
}
</style>