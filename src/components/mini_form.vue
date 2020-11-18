<template>
  <div class="mini_form">
      <h3>Pronto para planejar seu sossego?</h3>
      <br>
      <p>Agende uma consulta sem compromisso pelo formulário abaixo.</p>
      <br>
      <p>Nome:</p>
      <input type="text">
      <p>E-mail:</p>
      <input type="text">
      <p>Estado Civil:</p>
      <input type="text">
      <p>Profissão:</p>
      <input type="text">
      <p>Telefone/Whatsapp:</p>
      <input type="text">
      <p>Renda Mensal:</p>
      <input type="text">
      <br>
      <br>
      <div class="button">Enviar</div>
      <br>
  </div>
</template>

<script>
export default {
  name: 'MiniForm'
}
</script>
 <style>
 .mini_form{
    background: rgb(50,52,105);
    width: 350px; 
    margin-left: calc(70% - 205px); 
    margin-top: -250px;
    padding-top: 10px;
    padding-left: 30px;
    padding-right: 30px;
    font-weight: 900;
 }  
 .mini_form>h3{
    color: rgb(255,155,35);
    font-size: 34px;
 }
 .mini_form>p{
     font-size: 20px;
     color: white;
     font-weight: 100;
     margin:0px;
 }
 .mini_form>input[type="text"]{
     width: 100%;
     height: 30px;
     margin-bottom: 4px;
 }
 .mini_form>.button{
    width: 100px;
    height: 30px; 
    background: rgb(255,155,35);
    color: white;
    margin: auto;
    text-align: center; 
    border-radius: 20px;
    padding-top: 4px;
    padding-bottom: 2px;

 }

 @media screen and (max-width:900px){
.mini_form {
    width: 320px;
    margin-left: calc(50% - 160px);
    margin-top: 20px;
}

}

 </style>