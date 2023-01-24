# anidaacion
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selectores ,pseudo-clases y pseudo-elementos en css</title>
<link rel="stylesheet" href="css/ejercicioanidacion.css">
</head>
<body> 
        <button class="contenedor">pase por arriba</button>
    
</body>
</html>

body {
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height:100vh ;
    background-color:white;
}
        .btn-contenedor {
            text-transform: uppercase;
            color:#333;
            font-style: italic;
            background-color:#ddd;
        }
        .btn-contenedor:hover {
                /*se activa cuando el raton pasa por encima*/
                background-color:green;
        }
.btn-contenedor {
    position: relative;
    padding: 10px 20px;
    border-radius: 10px;
    border: none;
    color: white;
border-bottom: 10px  solid darkgreen;    
background-color: white;
cursor: pointer;
transition: background-color 150ms

}

/*.btn-tooltip:hover::before{
    content: "esto es un tooltip";
}*/
.contenedor{
    position: absolute;
    /*visibility: hidden;*/
    opacity: 0;
    top: -50px;
    left: -100%;
    transform: translateX(25%);
    color: #ddd;
    background-color: #333;
    padding: 5px 10px;
    border-radius: 5px;
    transition:opacity  all 150ms;
}

.btn-contenedor:hover .contenedor {
    /*visibility: visible;*/
    opacity: 1;
}

.contenedor::before{
    content: :;
}
