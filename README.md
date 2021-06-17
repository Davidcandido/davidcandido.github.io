<html>
  <head>
    <meta charset="utf-8">
    <link href="imagem/centralizar-imagem.css" rel="stylesheet" /> 
    <link href="estilos/cor-pagina.css" rel="stylesheet" />
    <link href="estilos/red.css" rel="stylesheet" />
     <link href="estilos/fonte.css" rel="stylesheet" />
    <link href="estilos/separando.css" rel="stylesheet" />
    <link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Open+Sans:sans-serif,300&display=swap" rel="stylesheet"> 
    <title>Minha página de teste</title>
  </head>
  <body>
  <h1> Nova York Moderna  </h1> 
<img src="imagens/novayork.jpeg" alt="nova york de cima">
 <p> Nova York virou uma vitrine do sucesso da vacinação nos EUA ao comemorar queda de 95% no número de casos por covid-19 e 24 horas sem nenhuma morte causada pelo coronavírus. A marca não era vista desde meados de março de 2020, quando o vírus começou a se espalhar no país. "É impressionante ver o progresso realizado", celebrou publicamente o prefeito, Bill de Blasio.</p>
    <p> Nessa cidade é possivel encontrar</p>
    <ul>
    <li>  engenheiros </li>
    <li> professores </li>
    <li> e enfermeiros </li>
    <p> <a href="https://www.correiobraziliense.com.br/mundo/2021/06/4929187-nova-york-tem-1-dia-sem-mortes-e-vira-vitrine-do-sucesso-da-vacinacao.html"> Nova York</a> chegou a registrar mais de 1 mil mortos por dia. O município tem a maior densidade populacional dos EUA, um desafio para as políticas de distanciamento social, e virou o epicentro da pandemia no país. 
    </p>
    <button>Mudar usuário</button>
  <script src="scripts/main.js"></script>
  </body>
let minhaImagem = document.querySelector('img');
minhaImagem.onclick = function() {
    let meuSrc = minhaImagem.getAttribute('src');
    if(meuSrc === 'imagens/firefox-icon.png') {
      minhaImagem.setAttribute ('src','imagens/firefox2.png');
    } else {
      minhaImagem.setAttribute ('src','imagens/firefox-icon.png');
    }
}

let meuBotao = document.querySelector('button');
let meuCabecalho = document.querySelector('h1');

function defineNomeUsuario() {
  let meuNome = prompt('Por favor, digite seu nome.');
  if(!meuNome || meuNome === null) {
    defineNomeUsuario();
  } else {
    localStorage.setItem('nome', meuNome);
    meuCabecalho.innerHTML = 'Mozilla é legal, ' + meuNome;
  }
}

if(!localStorage.getItem('nome')) {
  defineNomeUsuario();
} else {
  let nomeGuardado = localStorage.getItem('nome');
  meuCabecalho.textContent = 'Mozilla é legal, ' + nomeGuardado;
}

meuBotao.onclick = function() { defineNomeUsuario();
    
    img {
  display: block;
  margin: 0 auto;
}
    
    body {
  width: 600px;
  margin: 0 auto;
  background-color: #FF9500;
  padding: 0 20px 20px 20px;
  border: 5px solid black;
}
    
    h1 {
margin: 0;
  padding: 20px 0;
  color: #00539F;
  text-shadow: 3px 3px 1px black;

}
p, li {
  font-size: 16px;
  line-height: 2;
  letter-spacing: 1px;
  
    h1{
  font-size: 60px;
  text-align: center;
}

    html {
  background-color: #00539F;
}

    
    </html> 
