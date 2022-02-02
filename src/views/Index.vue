<template>
  <div class="home">
      <Navbar />
      <div class="banner" >
     <div class="escurecer"></div>
      <div class="main-card pt-5">
      
          <div class="content">
            <h1>Unlimited movies, TV <br>shows, and more.</h1>
            <h2>Watch anywhere. Cancel anytime.</h2>
          </div>
          <form action="" method="get">
            <h3>Ready to watch? Enter your email to create or restart your membership.</h3>
              <div class="input-group">
                <input type="text" class="form-control rounded-0" placeholder="Email Adress">
                <button class="btn  rounded-0 btn-danger" type="submit">Get started</button>
              </div>
          </form>   
        </div>
      </div>
    
      <section class="Onde-assistir d-flex justify-content-center align-items-center">
          <div class="row">
            <div class=" col-md-6 d-flex justify-content-center align-items-center">
              <div class="content">
                  <h1>Enjoy on your TV.</h1>
                  <h2>Watch on Smart TVs, Playstation, Xbox, Chromecast, Apple TV, Blu-ray players, and<br> more.</h2>
              </div>
            </div>
            <div class="col-md-6 d-flex justify-content-center align-items-center">
                <div class="video-content">
                    <img src="../assets/img/tv.png" alt="" srcset="">
                    <video  loop autoplay>
                      <source src="../assets/img/video-netflix.mp4" type="video/mp4">
                  </video>
              </div>
             </div>
          </div>
      </section>
      <section class="download d-flex justify-content-center align-items-center">
          <div class="row mb-4">
            <div class=" col-md-6 d-flex justify-content-center align-items-center">
              <div class="image position-relative">
                <img src="../assets/img/mobile.jpg" alt="Baixar series e filmes netflix" srcset="">
                <div class="second-image ">
                  <div class="image">
                    <img src="../assets/img/boxshot.png" alt="">
                  </div>
                  <div class="texto">
                    <h4>Stranger Things</h4>
                    <h4>Downloading...</h4>
                  </div>
                  <div class="gif">
                    <img src="../assets/img/download-icon.gif">
                  </div>
                  
                </div>
              </div>
            </div>
            <div class="col-md-6 d-flex justify-content-center align-items-center">
                <div class="content">
                  <h1>Download your shows to watch offline.</h1>
                  <h2>Save your favorites easily and always have something to watch.</h2>
              </div>
             </div>
          </div>
      </section>
      <section class="todo-lugar d-flex justify-content-center align-items-center">
          <div class="row">
            
            <div class="col-md-8 d-flex justify-content-end align-items-center">
                <div class="content">
                  <h1>Watch everywhere.</h1>
                  <h2>Stream unlimited movies and TV shows on your phone, tablet, laptop, and TV.</h2>
              </div>
             </div>
          </div>
      </section>
       <section class="kids d-flex justify-content-center align-items-center">
          <div class="row ">
            <div class=" col-md-6 d-flex justify-content-center align-items-center">
              <div class="image ">
                <img src="../assets/img/kids.png" alt="Baixar series e filmes netflix" srcset="">
               
              </div>
            </div>
            <div class="col-md-6 d-flex justify-content-center align-items-center">
                <div class="content">
                  <h1>Create profiles for kids.</h1>
                  <h2>Send kids on adventures with their favorite characters in a space made just for them—free with your membership.</h2>
              </div>
             </div>
          </div>
      </section>
      <section class="questions">
 
            <div class="accordion" id="accordionExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
        Accordion Item #1
      </button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        <strong>This is the first item's accordion body.</strong> It is shown by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
        Accordion Item #2
      </button>
    </h2>
    <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        <strong>This is the second item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingThree">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        Accordion Item #3
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        <strong>This is the third item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
      </div>
    </div>
  </div>
            </div>
          
      </section>
     
     
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'



export default {
  name: 'Home',
  components: {Navbar},
}
</script>
<style src="@/views/style2.scss" lang="scss" scoped></style>
