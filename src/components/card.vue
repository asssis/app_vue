<template>
  <div>
    <img src="https://i.picsum.photos/id/432/650/650.jpg?hmac=7cagJCe6jk-wwxN8Tvy4u5aqvNfIPAIP1WtUa_BFQNA">	
    <h3>{{ title }}</h3>
    <p>{{ body }}</p>
    <div class="button">Continuar</div>
  </div> 
</template>

<script>
export default {
  name: 'Card',
  props: { 
    title: String,
    body: String
  }
}
</script>
 <style>
  .card{
    border: 3px solid rgb(50,52,105);
    border-bottom: 80px solid  rgb(50,52,105);
    color: rgb(50,52,105);
    width: 350px;
    padding: 10px; 
    float: left;
    margin-left: 40px;
    margin-right: 40px;
    margin-bottom: 50px;
 }
 .card>div>img{
    width: calc(100% + 22px);
    height: 250px;
    margin-left: -11px;
    margin-right: -11px;
    margin-top: -11px; 
 }
 .card>div>p{
  font-size: 20px;
  color: rgb(50,52,105);
  min-height: 160px; 
 }
 .card>div>h3{ 
  color: rgb(50,52,105);
  font-size: 1.30em;
  min-height: 80px; 
 }
 .card>div>.button{
    width: 100px;
    height: 40px; 
    background: rgb(255,155,35);
    color: white; 
    text-align: center; 
    border-radius: 20px;
    padding-top: 10px;
    padding-bottom: 10px;
    position: relative;
    left: calc(50% - 50px);
    bottom: -74px;
    margin: 0px;
 }

 @media screen and (max-width:900px){
     .card{
    border: 3px solid rgb(50,52,105);
    border-bottom: 80px solid  rgb(50,52,105);
    color: rgb(50,52,105);
    width: 290px;
    padding: 10px; 
    float: left;
    margin-left: 10px;
    margin-right: 10px;
    margin-bottom: 50px;
 }
 }
 </style>