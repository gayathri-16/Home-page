<template>
  <div id="app">
<link href="https://fonts.googleapis.com/css2?family=Istok+Web:wght@700&family=Spartan:wght@300;500;800&display=swap" rel="stylesheet">
 <link href="https://fonts.googleapis.com/css2?family=Comfortaa:wght@300&display=swap" rel="stylesheet">
 <div id="nav" style="background:gray; width:500px;height:300px;"><NavigationMobile /> </div>
      
    <link  rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.14.0/css/all.css" />
    <div class="content" :class="{'open':showNav}">
   
    <div class="top-bar">
    <div id="navigation-icon" v-if="mobileView" @click="showNav = !showNav">
       <i class="fas fa-bars" v-if="showNav === false"></i>
        <i class="fas fa-times" v-if="showNav === true"></i>
   </div>
    <h1>Edie</h1>
      <Navigation v-if="!mobileView" style="margin-top:-1.5rem;"/>
    </div>
  <div id="home">
 <h6>Unhappy with your website?</h6>
 <h2>We create beatiful </h2> <br> <h2>and fast web services </h2>
   <div class="ex-image"><img src="./assets/photo2.jpg" alt=""></div> 
   <h3>Story,emotion </h3> <br>
    <h3> and purpose</h3>
    <p>We help transform your ideas into real  <br> world applications that will outperform  <br> your toughest competition and help you <br> achieve your strategic goals in short <br>
     period of time  </p>

     <label for="">Want us to contact you?</label> <br>
     <input type="text" class="email" placeholder="Email"> <span> <button>Join</button></span>
     <br>
     <br>
     <br>
  </div>
    
    <div id="service">
      <h4>We offer high</h4> <br> <h4>demand services</h4>
    
      <div class="design-type">
       <div class="ux-design">
         <button><i class="fas fa-pen"></i></button>
         <h5>UI/UX Design</h5>
         <p class="lorem">Lorem ipsum dolor sit amet, <br> consectetur adipisicing elit.Duis a <br> commodi consequatur maxime.  <br>
         Natus odio explicabo.</p>
         <button class="get-start">Get started</button>
       </div> 
      
       <div class="ux-design front-end">
         <button style="background-color:green;"><i class="fas fa-code"></i></button>
         <h5>Front-End</h5>
         <p class="lorem">Lorem ipsum dolor sit amet, <br> consectetur adipisicing elit.Duis a <br> commodi consequatur maxime.  <br>
         Natus odio explicabo.</p>
         <button class="get-start">Get started</button>  
       <i style="color:gray; font-size:30px;margin-left:8.5rem;" class=" fas fa-hand-pointer"></i>
       </div>
       
       
        <div class="ux-design back-end ">
         <button style="background-color:red;"><i class="fas fa-bars"></i></button>
         <h5>Back end</h5>
         <p class="lorem">Lorem ipsum dolor sit amet, <br> consectetur adipisicing elit.Duis a <br> commodi consequatur maxime.  <br>
         Natus odio explicabo.</p>
         <button class="get-start">Get started</button>
       </div>

      </div>
      <br><br><br> <br><br><br>

      <div id="ourwork">
        <h4 class="good">Good design means</h4> <br>
         <h4>good business</h4>
         <div class=" images "><img class="photo" src="./assets/photo4.jpg" alt=""><p class="title">Full stack application</p> <h3 class="smart">Smart home dashboard</h3> </div>
         <div class="images on-board"><img class="photo1" src="./assets/photo7.jpeg" alt=""><p class="title">UX/UI design</p> <h3 class="smart">Onboard application</h3> </div>
         <div class=" images" id="book"><img class="photo" src="./assets/booking.png" alt=""><p class="title">Mobile application</p> <h3 class="smart">Booking system</h3> </div>
         <div class="on-board" id="juice" ><img class="photo1" src="./assets/soft drink.png" alt=""><p class="title">Front End application</p> <h3 class="smart">Juice product homepage</h3> </div>
        
      </div>
       <h4 class="see">see more  <i style="color:rgb(16, 180, 245); font-size:12px;" class=" fas fa-arrow-right"></i></h4>
    </div> 
    <br>
<div class="ourwork">
  <h6 class="meet" style="">Meet the team</h6>
  <h4>We are chilled</h4> <br>
 <h4>and a laidback</h4>  <br> <h4> team</h4>
  <p class="ipsum" style="">Lorem ipsum dolor sit amet, <br> consectetur adipisicing elit. </p>
  
  <div class="worker">
     <div><img class="people image2" src="./assets/image2.jpg" alt=""></div>
    <div><img class="people image3" src="./assets/image3.jpg" alt=""></div>
    <div><img class="people image1" src="./assets/image1.jpg" alt=""></div>
  </div>
  <br><br><br><br><br>
<div id="client">
  <h1 class="about-company">"Fast and outstanding results. Edie understands <br> thier customer's need. They have a young and <br>talented team."</h1>
  <img class="carlos" src="./assets/designer.jpg" alt="">
  <h2 class="d-name">Carlos tran</h2>
  <p class="d-about">The Decorate Gatsby</p>
</div>
</div>
<br><br> <br> 
  
  <div id="footer">
    <ul class="link">
      <li class="list"> <a href="#home"> Home</a></li>
       <li class="list"> <a href="#service"> Service</a></li>
        <li class="list"> <a href="#ourwork"> Ourworks</a></li>
         <li class="list"> <a href="#client"> Clients</a></li>
          <li class="list"> <a href="#footer"> Contact</a></li>
    </ul>
    <h1 class="author">Edie</h1>
    <div id="icon">
   <i class="fab fa-instagram" style="filter:index(0);"></i>
   <i class="fab fa-google-plus-square" style="color:white;"></i>
   <i class="fab fa-twitter-square"></i>
   </div>
 <h4 class="contact">Want us contact you?</h4>

<input type="text" class="email detail"  placeholder="Email" name="" id=""> <button style="margin-left:-4.2rem;">join</button>
  
   </div>
   </div>
   
</div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import NavigationMobile from './components/NavigationMobile.vue'

export default {
  data: ()=>{
    return{
      mobileView:true,
      showNav:false
    };
  },
methods:{
  handleView(){
    this.mobileView = window.innerWidth <= 575;
  }
},
  components: {
    Navigation,
    NavigationMobile
  },
  created(){
     this.handleView();
     window.addEventListener('resize',this.handleView);
  }
};
</script>

<style>
body{
  width:100%;
  height:100vh;
  margin:0;
  padding:0;
  font-family:"Segoe UI", Tahoma;

}
#app {
  position:relative;
  width:calc(100% - 10px);
  height:calc(100vh - 20px);
  margin-top:-8rem;
  
 }
.top-bar{
  display:flex;
  width:500px;
}
h1{
  text-align:left;
  margin-top:2rem;
  color:rgb(44, 43, 43);
}
h6{
margin-left: 20rem;
color:rgb(77, 199, 247);
font-size:18px;
letter-spacing: 1px;
font-family: 'Poppins',sans-serif;
}
h2{
margin-left: 20rem;
font-family: 'Comfortaa', cursive;
margin-top:-2rem;
margin-bottom:1rem;
font-size:36px;
color:rgb(46, 44, 44);
letter-spacing: 1px;
word-spacing: 2px;
font-weight:bold;


}
h3{
  margin-left: 20rem;
font-family: 'Istok Web', sans-serif;
margin-top:1.5rem;
margin-bottom:-2rem;
font-family: 'Comfortaa', cursive;
font-size:36px;
color:rgb(46, 44, 44);
letter-spacing: 1px;
word-spacing: 2px;
font-weight:bold;
}
h4{
  margin-left: 12rem;
font-family: 'Istok Web', sans-serif;
margin-top:-1rem;
margin-bottom:0.4rem;
font-family: 'Comfortaa', cursive;
font-size:36px;
color:rgb(46, 44, 44);
letter-spacing: 1px;
word-spacing: 2px;
font-weight:bold;
}

p{
  margin-top:4rem;
  margin-left:20rem;
  
  color:rgb(27, 27, 27,0.8);
}
#navigation-icon{
  padding:10px 10px 20px;
   cursor:pointer;
}
#navigation-icon i{
  font-size:2rem;
  float:right;
  margin-left:25rem;
}
.content{
  position:absolute;
  top:10px;
  width:calc(100% - 50px);
  height:calc(100vh - 60px);
  padding:30px;
  margin-top:-1rem;
  background-color:#fff;
  transition:1s transform cubic-bezier(0,.12,.14,1);

}.open{
  transform: translateY(280px);
}
.ex-image{
  align-items: center;
 
  
}
.ex-image img{
  border-radius:15px;
  margin-left:5rem;
  width:85rem;
  height:300px;
  margin-top:1.5rem;
}
label{
  margin-left:20rem;
  font-family: 'Krub', sans-serif;
  color:rgb(65, 64, 64,0.7);
  font-size:14px;

}
.email{
  margin-left:20rem;
  margin-top:0.5rem;
  width:180px;
  height:40px;
  border-radius:10px;
  border-style:none;
  background-color: rgb(228, 220, 220);
}
::-webkit-input-placeholder{
    font-size:14px;
    padding:1.5rem;
    color:rgb(146, 144, 144);
    font-family: 'Comfortaa', cursive;
  }
button{
  margin-left:1rem;
  background:rgb(29, 146, 192);
  border-style:none;
  border-radius:10px ;
  width:60px;
  height:35px;
  color:white;
  font-size:13px;
  font-family: 'Comfortaa', cursive;
}
.design-type{
  width:100%;
 
 
}
.ux-design{
  width:18%;

  margin-left:13rem;
  align-items: center;
  padding:10px 30px 10px;
  margin-top:1rem;

}
.front-end{
  margin-left:37rem;
  margin-top:-21.7rem;
   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
.back-end{
  margin-left:61rem;
  margin-top:-21.7rem;
}
.ux-design button{
  width:50px;
  height:50px;
  background:rgb(29, 146, 192);
   margin-top:5rem;
   margin-left:0.2rem;;
 
}
.ux-design button i{
  color:white;
  font-size:18px;
 
}
.ux-design h5{

color:rgb(39, 39, 39);
font-size:18px;
letter-spacing: 1px;
font-family: 'Poppins',sans-serif;
}
.ux-design .get-start{
  width:100px;
  height:30px;
  background: rgb(236, 236, 236);
  color:gray;
  margin-top:1rem;
  margin-left:-0.4rem;
}
.ux-design .lorem{
  margin-left:-0.1rem;
  margin-top:-1rem;
}
#hand{
  margin-left:5rem;
  color:gray;


}
.images{
  width:500px;
  height:500px;
  border-radius:20px;
  background: rgb(247, 85, 85);
  margin-left:11rem;
  margin-top:12rem;
  margin-bottom:10rem;

}
.photo{
  width:500px;
  height:500px;
border-radius:25px;
}
 .on-board{
  margin-top:-50rem;
  margin-left:50rem;
 
  
}
.photo1{
  border-radius:25px;
  width:500px;
  height:500px;
}
#book {
  margin-top:18rem;
  }
  #juice{
  margin-top:-50rem;
}
.title{
  color:gray;
  margin-top:0.5rem;
  font-size:14px;
  margin-left:1rem;

}
.smart{
  margin-top:-0.1rem;
  font-size:20px;
  margin-left:1rem;
  font-weight: bold;
  font-family:'Poppins',sans-serif

}
.see{
  font-size:16px;
  color:rgb(16, 180, 245);
  margin-left:75rem;
 margin-top:10rem;
 font-weight: bolder;

}
.worker{
  width:500px;
  height:500px;
 margin-top:-20rem;
  margin-left:58rem;
 
}
.people
{
  width:200px;
  height:200px;
  border-radius:15px;
}


.image1{
  margin-left:10rem;
  margin-top:-4rem;

}
.image2{
    margin-left:10rem;
    margin-top:4rem;
    margin-bottom:-8rem;

}
.image3{
  margin-left:-3.5rem;
}
.about-company{
  margin-left:12rem;
  margin-top:-2rem;
  font-weight: bold;
  font-size:30px;
font-family: 'Comfortaa', cursive;
word-spacing: 5px;
line-height: 40px;
color:black;

}
.d-name{
  font-size:16px;
  margin-top:-4rem;
  margin-left:18rem;
  font-family: 'Comfortaa', cursive;
  font-weight: 700px;
  color:black;
}
.d-about{
  margin-top:-0.5rem;
   margin-left:18rem;

}
.carlos{
  width:75px;
  height:75px;
  border-radius: 5px;
  margin-left:12rem;
  margin-top:0.5rem;
}
#footer{
  width:100%;
  background:black;
  height:400px;
  padding: 10px 20px 10px;
  margin-left:-1.5rem;
  
}


ul{
  list-style: none;
  display: block;
  margin-top:5rem; 
  
  
}
.list{
  margin-top:3rem;
}
.list a{
  text-decoration: none;
  font-size:20px;
  font-family:'Poppins', sans-serif;
  line-break: 1px;
  color:rgb(255, 255, 255);
  letter-spacing: 1px;
  font-weight: lighter;
  display:block;
  margin-left:-45rem;
 margin-top:1rem;

  
}
.author{
  margin-left:28rem;
  margin-top:-13rem;
  color:white;
}

.contact{
  margin-top:-5rem;
margin-left:60rem;
  font-size:12px;
  color:white;
}
.detail{
  margin-left:60rem;
  width:220px;
}
#icon{
  margin-left:27rem;
  margin-top:-0.5rem;
}
#icon i{
  color:white;
  margin-left:1rem;
  font-size:24px;
  cursor:pointer;
}
.meet{
  color:red;
   margin-left:12rem;
}
.ipsum{
  margin-left:12rem; 
  margin-top:-0.1rem;
}
@media only screen and (max-width:550px){
  #app {
 width:100%;
 height:auto;
margin-top:-2rem;
  
 }
.top-bar{
  display:flex;
  width:100%px;
}
h1{
  text-align:left;
  margin-left:-24.3rem;
  margin-top:0rem;
 margin-bottom: 2rem;
}
h6{
margin-left: 4rem;
margin-top:0.5rem;
}
h2{
margin-left: 4rem;
margin-top:1rem;
margin-bottom:-1.5rem;
font-size:25px;
}
h3{
margin-left: 4rem;
margin-top:1.5rem;
margin-bottom:-1.8rem;
font-size:25px;

}
h4{
margin-left: 4rem;
margin-top:-1rem;
margin-bottom:0.4rem;
font-size:25px;
}

p{
  margin-top:4rem;
  margin-left:4rem;
 }
#navigation-icon{
   
   cursor:pointer;
}
#navigation-icon i{
  font-size:2rem;
  float:right;
  margin-left:23rem;
  margin-top:rem;
}
.content{
  position:absolute;
  top:10px;
  width:calc(100% - 50px);
  height:calc(100vh - 60px);
  padding:30px;
  margin-top:-1rem;
  background-color:#fff;
  transition:1s transform cubic-bezier(0,.12,.14,1);

}.open{
  transform: translateY(280px);
}
.ex-image{
  align-items: center;
 
  
}
.ex-image img{
  border-radius:15px;
  margin-left:-0.5rem;
  width:28rem;
  height:290px;
  margin-top:2.5rem;
}
label{
  margin-left:4rem;
  font-size:14px;
}
.email{
  margin-left:4rem;
  margin-top:0.5rem;
}
.design-type{
  width:100%;
 }
.ux-design{
  width:60%;
  margin-left:4rem;
  align-items: center;
  padding:10px 30px 10px;
  margin-top:-2.5rem;

}
.front-end{
  margin-left:4rem;
  margin-top:1rem;
   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
.back-end{
  margin-left:4rem;
  margin-top:.7rem;
}
.ux-design button{
  width:50px;
  height:50px;
  background:rgb(29, 146, 192);
   margin-top:3rem;
   margin-left:0.2rem;;
 
}

.good{
  margin-top:-5rem;
}

.images{
  width:300px;
  height:300px;
  border-radius:20px;
  background: rgb(247, 85, 85);
  margin-left:4rem;
  margin-top:5rem;
  margin-bottom:15rem;

}
.photo{
  width:300px;
  height:300px;
border-radius:25px;
}
 .on-board{
  margin-top:-8rem;
  margin-left:4rem;
   
}
.photo1{
  border-radius:25px;
  width:300px;
  height:300px;
}
#book {
  margin-top:-7rem;
  }
  #juice{
  margin-top:-7rem;
}

.see{
 margin-left:5rem;
 margin-top:3.5rem;
 
}
.meet{
  margin-left:4rem;
  margin-top:2rem;
}
.ipsum{
  margin-left:4rem;
  margin-top:1rem;
}
.worker{
  width:400px;
  height:400px;
 margin-top:-1rem;
  margin-left:4rem;
 
}
.people
{
  width:200px;
  height:200px;
  border-radius:15px;
}


.image1{
  margin-left:10rem;
  margin-top:-4rem;

}
.image2{
    margin-left:10rem;
    margin-top:4rem;
    margin-bottom:-8rem;

}
.image3{
  margin-left:-3.5rem;
}
.about-company{
margin-left:2rem;
margin-top:3rem;
font-weight: bold;
font-size:26px;

}
.d-name{
  font-size:16px;
  margin-top:-4rem;
  margin-left:10rem;
 
}
.d-about{
  margin-top:1.8rem;
   margin-left:10rem;

}
.carlos{
  width:75px;
  height:75px;
  border-radius: 5px;
  margin-left:4rem;
  margin-top:0.5rem;
}
#footer{
  width:100%;
  background:black;
  height:auto;
  padding: 10px 20px 10px;
  margin-left:-1.5rem;
  
}


ul{
  list-style: none;
  display: block;
  margin-top:2rem; 
  
  
}
.list{
  margin-top:3rem;
}
.list a{
  
  margin-left:-52rem;
  margin-top:1rem;

  
}
.author{
  margin-left:2rem;
  margin-top:3rem;
  color:white;
}

.contact{
  margin-top:2rem;
margin-left:2rem;
  font-size:12px;
  color:white;
}
.detail{
  margin-left:1rem;
  width:220px;
}
#icon{
  margin-left:1rem;
  margin-top:-1rem;
}
#icon i{
  color:white;
  margin-left:1rem;
  font-size:24px;
  cursor:pointer;
}

}
</style>
