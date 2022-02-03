<template>
  <form action="" method="get">
            <h3>Ready to watch? Enter your email to create or restart your membership.</h3>
              <div class="input-group">
                <input type="text" class="form-control rounded-0" placeholder="Email Adress">
                <button class="btn  rounded-0 btn-danger" type="submit">Get started</button>
              </div>
    </form>  
</template>

<script>
export default {
        name: 'FormCad'
}
</script>

<style lang="scss" scoped>
    form{
           
            h3{
                font-size: var(--font-size-3);
                margin:2rem 0 1.5rem 0;
            }
            .input-group{
                height: 3.8rem;
                

                input{
                    height: 100%;
                    font-size: var(--font-size);
                    color: #000 !important;
                    font-weight: 500;
                    border-radius: .1rem 0 0 .1rem !important;
                   
                }
                 button{
                    height: 100%;
                    font-size: var(--font-size-3);
                    border-radius: 0 .2rem .2rem 0 !important;
                 }
 
            }
        }
</style>