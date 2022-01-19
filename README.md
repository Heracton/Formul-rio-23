<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=Edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="style.css">
  <title>Formulário da clinica</title>
  <!-- Custom Styles -->  
<style>
  body {
    font-family: Arial, Helvetica, sans-serif; 
    background-image: linear-gradient(45deg, #ACAD28, #959532, #FFFF00); 
  } 
    .box {
      color: white; 
      position: absolute;
      top: 50%; 
      left: 50%; 
      transform: translate(-50%, -50%); 
      background-color: rgba(0, 0, 0, 0.6); 
      padding: 15px;
      border-radius: 15px; 
      width: 20%; 
    } 
      fieldset {
        border: 3px solid #FBFD00BF; 
    } 
    legend {
      border: 1px solid #FBFD00BF; 
      padding: 10px; 
      text-align: center; 
      background-color: #FBFD00BF; 
      border-radius: 8px; 
    }
    .inputBox {
      position: relative; 
    }
    .inputUser {
      background: none; 
      border: none; 
      border-bottom: 1px solid white; 
      outline: none; 
      color: white; 
      font-size: 15px; 
      width: 100%; 
      letter-spacing: 2px;
    } 
    .labelInput {
      position: absolute; 
      top: 0px; 
      left: 0px; 
      transition: -5px; 
    } 
    
    } 
    #data_cliente {
      border: none; 
      padding: 8px; 
      border-radius: 10px; 
      outline: none; 
      font-size: 15px; 
    }
    #submit{
      background-image: linear-gradient(45deg, #F4F700, #A7A81D, #AEAF46); 
      width: 100%; 
      border:none; 
      padding: 15px; 
      color: white; 
      font-size: 15px; 
      cursor: pointer; 
      border-radius: 10px;
    }
      legend {
        box-shadow: -1px -1px lightyellow;
      }
  </style>
  </head>

<body>
  <div class="box"> 
  <form action="">
   <fieldset>
     <legend><b>Formulário de cliente</b></legend> 
     <br> 
     <div class="inputBox"> 
       <input type="text" name="nome" id="nome" class="inputUser" required> 
       <label for="nome">Nome do paciente</label>
     </div>  <!--nome do paciente-->
     <br> <br>
     <div class="inputBox">
       <select name="procedimento" id="procedimento" class="inputUser" required>
          <option selected disabled value="">Selecione uma opção</option>
          <option>BOTOX</option>
          <option>FIOS DE PDO</option>
          <option>SKIN BOOSTER</option> 
          <option>LIPO DE PAPADA</option>
          <option>MICROAGULHAMENTO</option>
          <option>PREENCHIMENTO LABIAL</option>
          <option>PREENCHIMENTO FACIAL</option>
          <option>SCULPTRA PARA BUMBUM</option>
          <option>INTRADERMOTERIA CAPILAR</option>
          <option>REJUVENECIMENTO DAS MÃOS</option>
           <option>BIOSTIMULADOR DE COLÁGENO</option>
       </select>
       <label for="procedimento">Procedimento</label>
     </div> <!-- procedimento-->
     <br> <br>
     <div class="inputBox">
       <input type="text" name="numero" id="numero" class="inputUser" required>
       <label for="numero" >Número de sessões</label>
     </div> <!--numero de sessões-->
       <p>Sexo:</p> 
      <input type="radio" id="feminino" name="genero" value="faminino" required> 
      <label for="Feminino">Feminino</label> 
      <br>
      <input type="radio" id="masculino" name="genero" value="masculino" required> 
      <label for="masculino">Masculino</label> 
      <br>
      <input type="radio" id="outro" name="genero" value="outro" required>
      <label for="outro">Outro</label> 
      <br> <br>
        <label for="data_cliente"><b>Data do cliente</b></label>
        <input type="date" name="data_cliente" id="data_cliente"required> 
     <br> <br>
     <div class="inputBox"> 
      <input type="text" name="valor" id="valor" class="inputUser" required> 
      <label for="valor">Valor</label> 
     </div> 
     <br> <br>
     <input type="submit" name="submit" id="submit">
    </fieldset> 
  </form>
  </div>
</body>
</html>
