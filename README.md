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

* {
    padding: 0;
    margin: 0;
}

.contenedor {
    width: 200px;
    height: 100px;
    background-color: white;
}
.contenedor:hover {
        /*se activa cuando el raton pasa por encima*/
        font-style: italic;
        background-color: green;
        text-transform: 3s;
        

}


.contenedor:visited {
    color: white;
}
.contenedor:hover {
    color: white;
}
.contenedor:active {
    opacity: 0%;
    transition: 2s;
}

.contenedor:hover::before{
    content: "¡Hecho!";
    opacity: 200%;
}


