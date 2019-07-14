# Curso-PHP
Código HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link href="https://fonts.googleapis.com/css?family=Oswald:200,300,400,500,600,700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="assets\css\estilo.css">
    <title>Curso PHP</title>
</head>
<body>
   <header class="cabecalho">
       <h1>Curso PHP</h1>
       <h2>Índice dos Exercicíos</h2>
   </header>
   <main class="principal">
       <div class="conteudo">
           
       </div>        
   </main>
   <footer class="rodape">
       COD3R & ALUNOS © 2019
   </footer>
</body>
</html>

Css
* {
    font-family: 'Oswald', sans-serif;
    box-sizing: border-box;
}

body {
    height: 100vh;
    margin: 0px;
    display: grid;
    grid-template-rows: 120px 1fr 60px;
    grid-template-columns: 1fr;
    grid-template-areas: 
        "cabecalho" 
        "principal" 
        "rodape";   
}

.cabecalho {
    grid-area: cabecalho;
    background-color: #1867c0;
    collor: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 10px;
    z-index: 1;
    box-shadow: 0px 4px 9px -2px rgba(0,0,0,0.75);
}

.cabecalho > h1 {
    margin: 0px;
    font-weight: 300;
    font-size: 2.8rem;
}

.cabecalho > h2 {
    margin: 0px;
    font-weight: 200;
    font-size: 1.6rem;
}

.principal {
    grid-area: principal;
    height: calc(100vh - 180px);
    background-color: #f0f0f0;
    padding: 20px;
}

.conteudo {
    position: relative;
    height: 100%;
    overflow-y: scroll;
    background-color: #fff;
    padding: 20px; 
}

.rodape {
    grid-area: rodape;
    background-color: #fff;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    font-size: 1.2rem;
    padding-right: 20px;
    color: #444;
    position: sticky;
    bottom: 20px;    
}
    
