

<template>
  <div> 
    <img class="topo" src="https://i.picsum.photos/id/432/650/650.jpg?hmac=7cagJCe6jk-wwxN8Tvy4u5aqvNfIPAIP1WtUa_BFQNA" alt="Minha Figura">	
     <div class="bem_estar"  data-aos="fade-right">
      <h4>Vida Toda</h4>
      <h1>BEM ESTAR</h1>
      <p>Soluções completas para viver mais e melhor.</p>
      <div class="button">Quero uma consultoria</div>
     </div>
     <MiniForm/>
     <div class="aling-left">
        <h3>Pense nisso...</h3>
        <p> O quanto o diagnóstico de uma doença grave, internação ou cirugia inesperada pode afetar, hoje, sua vida pessoal e financeira?</p>
      </div>
     <div class="blog">
        Blog
     </div>
  </div>
</template>

<script>

import MiniForm from './mini_form' 
export default {
  name: 'Body',
  components: {
    MiniForm
  }, 
}
</script>
 
<style>
 .topo{
     width: calc(100% + 10px);
     height: 660px;
    position: absolute;
    left: 0;
    bottom: 0;
    top: 0;
    z-index: -100;
 }
 .bem_estar{
    border: 3px solid rgb(50,52,105);
    color: rgb(50,52,105);
    width: 350px;
    padding: 10px;
    margin-top: 100px;  
   margin-left: 30px;
   
 }
 .bem_estar>h1{
    font-size: 88px;
    margin-top: 10px;
    line-height: 110px;
    font-weight: 900;    
 }
 .bem_estar>h4{
    margin-top: 40px;
    margin-bottom: -26px;
    padding-left: 3px;
    font-size: 30px;
 }
 .bem_estar>p{
    margin-top: 110px;
    margin-bottom: 70px;
    padding-left: 3px;
    font-size: 29px;
    font-weight: 600;
 }
 .bem_estar>.button{
    width: 100%;
    background: rgb(255,155,35);
    border: none;
    color: white;
    font-size: 25px;
    padding-top: 10px;
    padding-bottom: 15px; 
    text-align: center;
    text-decoration: none;
    display: inline-block; 
    margin-bottom: 30px;
 } 
  
 
.blog{
   background:  rgb(50,52,105);
   width: 420px;
   height: 80px;
   margin-top: 20px;
   margin-left: -10px;
   color: white;
   font-size: 50px;
   text-align: center;
   padding-top: 10px;
   padding-bottom: 25px;
}
.aling-left{
    width: 400px;
    padding-left: 70px;
    text-align: justify;
}
.aling-left>h3{
   color:rgb(255,155,35);
   font-size: 30px;
}
.aling-left>p{
   width: 340px;
   font-size: 20px;
   color:  rgb(50,52,105);
}

 @media screen and (max-width:900px){
  .bem_estar {
    width: 300px;
    margin-left: calc(50% - 150px);
    margin-top: 2px;
}
.bem_estar>h1{
   
    font-size: 75px;
}
.bem_estar>p{
   
    margin-top: 65px;
}
   .blog{  
     width: 377px;
     margin-left: calc(50% - 188px);
     margin-top: 140px;
   }
   .aling-left{
     width: 350px;
     margin-left: 5px;
     height: 50px; 
     text-align: center; 
     margin-top: 100px;
     text-align: center;
     padding: 0px;
   } 

   .aling-left>p{
   width: 275px;
   font-size: 20px;
   padding-left: 0px;
   padding-right: 0px;
   margin: auto;
   margin-top: 20px;
   color:  rgb(50,52,105);
}

}
 </style>