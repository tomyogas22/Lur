# Lur
<!DOCTYPE html>
<html>
<head>
    <title>Programa para salir de la friendzone</title>
    <meta charset="UTF-8">
</head>
<style>
    *{
        margin: 0px;
        padding: 0px;
    }
    body{
        background: #fcfcfc;
    }
    .contenedor {
        margin: auto;
        width: 900px;
        margin-top: 300px;
        text-align: center;
    }
    .titulo{
        margin-bottom: 20px;
    }
    .opciones p {
        background: #ffa02a;
        display: initial;
        padding: 12px;
        color: #ffffff;
        border-radius: 2px;
        font-weight: bold;
    }
    p.p1 {
        position: absolute;
        top: 400px;
        left: 609px;
        width: 100px;
    }
    p.p2{
        position: absolute;
        top: 400px;
        left: 800px;
        width: 100px;
    }
    #si {
        background: #515050;
        left: 420px;position: absolute;
        top: 122px;
        width: 550px;
        color: #ffffff;
        padding: 50px;
        display: none;
    }
</style>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
<script>
$(document).ready(function(){
  $(".p1").hover(function(){
      arriba =  Math.random() * (400 - 1) + 1;
      abajo =  Math.random() * (609 - 1) + 1;
    $(this).css("top", arriba);
    $(this).css("left", abajo);
    });
});
function dijoSi(){
    document.getElementById("si").style.display = "block";
}
</script>
<body>
<div class="contenedor">
    <div class="titulo">
        <h1>¿ME DAS UN BESO?</h1>
    </div>
    <div class="opciones">
        <p class="p1">NO</p>
        <p onclick="dijoSi()" class="p2">SI</p>
        <div id="si">    
                <img src="Memecorazon.jpg" width="70%">
                <h2>Yo sabia, veni bb que te lo doy</h2>
        </div>
    </div>
</div>
</body>
</html>
