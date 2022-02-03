<template>
  <div class="home">
      <Navbar :home="false" />
      <div class="banner" >
     <div class="escurecer"></div>
      <div class="main-card pt-5 px-4">
      
          <div class="content">
            <h1>Unlimited movies, TV <br>shows, and more.</h1>
            <h2>Watch anywhere. Cancel anytime.</h2>
          </div>
           <form-cad class="text-center mt-2"></form-cad>
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
                   
                    <video  loop autoplay @contextmenu.prevent>
                      <source src="../assets/img/netflix.mp4" type="video/mp4">
                  </video>
              </div>
             </div>
          </div>
      </section>
      <section class="download d-flex justify-content-center align-items-center">
          <div class="row mb-4">
            <div class=" col-md-6 mb-3 d-flex justify-content-center align-items-center">
              <div class="image position-relative bg-danger">
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
                <div class="content my-4">
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
      <section class="questions d-flex justify-content-center align-items-center flex-column w-100 ">
        <h1>Frequently Asked Questions</h1>
          <div class="row w-100  d-flex justify-content-center">
            <div class="col-md-10">
              <Cardfaq :cards="cards" />
            </div>
            <div class="col-md-7 my-4 mb-5">
              <form-cad class="text-center"></form-cad>
            </div>
          </div>   
      </section>
     

     <footer class="pt-5" >
       <div class="container text-sm-center">
          <div class="row  py-4 ml-3  text-md-left">
            <div class="col-md-12 my-2">
              <h5>Questions? Contact us.</h5>
            </div>
            <div class="col-md-6 col-lg-3 col-xl-3 mx-auto mt-3 ">
              <ul class="list-unstyled  ">
                  <li><a href="#">FAQ</a></li>
                  <li><a href="#">Investor Relations</a></li>
                  <li><a href="#">Privacy</a></li>
                  <li><a href="#">Speed Test</a></li>
              </ul>
            </div>
            <div class="col-md-6 col-lg-3 col-xl-3  mt-3  ">
                <ul class="list-unstyled ">
                  <li><a href="#">Help Center</a></li>
                  <li><a href="#">Jobs</a></li>
                  <li><a href="#">Cookie Preferences</a></li>
                  <li><a href="#">Legal Notices</a></li>
                </ul>
            </div>
            <div class="col-md-6 col-lg-3 col-xl-3 mx-auto mt-3 ">
                <ul class="list-unstyled ">
                  <li><a href="#">Account</a></li>
                  <li><a href="#">Ways to Watch</a></li>
                  <li><a href="#">Corporate Information</a></li>
                  <li><a href="#">Only on Netflix</a></li>
                </ul>
            </div>
            <div class="col-md-6 col-lg-3 col-xl-3 mx-auto mt-3 ">
                <ul class="list-unstyled ">
                  <li><a href="#">Media Center</a></li>
                  <li><a href="#">Terms of Use</a></li>
                  <li><a href="#">Contact Us</a></li>
                
                </ul>
            </div>
              <div class="col-md-12 my-2">
              <h6 >Netflix Angola</h6>
            </div>
          </div>
       </div>
     </footer>
     
      </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Cardfaq from '@/components/Card-faq.vue'
import FormCad from '@/components/Form-cad.vue'




export default {
  name: 'Home',
  components: {Navbar,Cardfaq,FormCad},
  data(){
    return{
      cards: [
        {id:1 , titulo: 'What is Netflix?',descricao:"Netflix is a streaming service that offers a wide variety of award-winning TV shows, movies, anime, documentaries, and more on thousands of internet-connected devices. You can watch as much as you want, whenever you want without a single commercial – all for one low monthly price. There's always something new to discover and new TV shows and movies are added every week!" },
        {id:2 , titulo:"How much does Netflix cost?" , descricao: "Watch Netflix on your smartphone, tablet, Smart TV, laptop, or streaming device, all for one fixed monthly fee. Plans range from USD3.99 to USD11.99 a month. No extra costs, no contracts."},
        {id:3 , titulo:"Where can I watch?" , descricao: "Watch anywhere, anytime. Sign in with your Netflix account to watch instantly on the web at netflix.com from your personal computer or on any internet-connected device that offers the Netflix app, including smart TVs, smartphones, tablets, streaming media players and game consoles. You can also download your favorite shows with the iOS, Android, or Windows 10 app. Use downloads to watch while you're on the go and without an internet connection. Take Netflix with you anywhere."},
        {id:4 , titulo:"How do I cancel?" , descricao: "Netflix is flexible. There are no pesky contracts and no commitments. You can easily cancel your account online in two clicks. There are no cancellation fees – start or stop your account anytime."},
        {id:5 , titulo:"What can I watch on netflix?" , descricao: "Netflix has an extensive library of feature films, documentaries, TV shows, anime, award-winning Netflix originals, and more. Watch as much as you want, anytime you want."},
        {id:6 , titulo:"Is netflix good for kids?" , descricao: "The Netflix Kids experience is included in your membership to give parents control while kids enjoy family-friendly TV shows and movies in their own space.Kids profiles come with PIN-protected parental controls that let you restrict the maturity rating of content kids can watch and block specific titles you don’t want kids to see."},
      ]
    }
  }
}
</script>
<style src="@/views/style2.scss" lang="scss" scoped></style>
