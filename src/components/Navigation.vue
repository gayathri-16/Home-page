<template>
  <div id="navigation">
   <link href="https://fonts.googleapis.com/css2?family=Encode+Sans:wght@300;400&family=Istok+Web:wght@700&family=Spartan:wght@300;500;800&display=swap" rel="stylesheet">
<ul class="nav-list" > 
     <li><a href="#home">Home</a></li> 
     <li><a href="#service">Service</a></li>
     <li><a href="#ourwork">OurWork</a></li>
     <li><a href="#client">Client</a></li>
     <li><a href="#footer">Contact</a></li>
   </ul>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style>
#navigation{
  display:flex;
  width:100%;
 
}
ul{
list-style: none;
margin-left:50rem;


}
 li {
 display: inline;

 }
 li a{

    text-decoration: none;
    padding:0px 25px 0px;
    color:rgb(56, 54, 54);
    font-weight:bold;
    font-size:18px;
  font-family: 'Encode Sans', sans-serif;
  letter-spacing: 1px;
    
 }


</style>