<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Gerador de Imagens</title>

<style>

*{
    box-sizing:border-box;
    margin:0;
    padding:0;
    font-family:Arial,sans-serif;
}

body{
    background:#f5f5f5;
    padding:20px;
}

.container{
    max-width:1000px;
    margin:auto;
    background:white;
    padding:20px;
    border-radius:12px;
    box-shadow:0 4px 12px rgba(0,0,0,.1);
}

h1{
    margin-bottom:20px;
}

.grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:15px;
}

label{
    display:block;
    margin-bottom:5px;
    font-weight:bold;
}

input{
    width:100%;
    padding:10px;
    border:1px solid #ccc;
    border-radius:6px;
}

button{
    padding:12px 20px;
    border:none;
    border-radius:8px;
    cursor:pointer;
    background:#0078d4;
    color:white;
    font-size:16px;
}

button:hover{
    background:#005fa3;
}

.canvas-area{
    margin-top:30px;
    text-align:center;
}

canvas{
    border:1px solid #ddd;
    max-width:100%;
}

.actions{
    margin-top:20px;
    display:flex;
    gap:10px;
    flex-wrap:wrap;
}

@media(max-width:768px){

.grid{
    grid-template-columns:1fr;
}

}

</style>
</head>
<body>

<div class="container">

<h1>Gerador de Imagens para Seat Map</h1>

<div class="grid">

<div>
<label>Texto</label>
<input id="textInput" value="AO">
</div>

<div>
<label>Tamanho da Imagem (px)</label>
<input id="sizeInput" type="number" value="256">
</div>

<div>
<label>Cor de Fundo</label>
<input id="bgInput" value="FFFFFF">
</div>

<div>
<label>Cor da Letra</label>
<input id="textColorInput" value="333333">
</div>

<div>
<label>Nome da Imagem</label>
<input id="fileNameInput" placeholder="imagem">
</div>

<div>
<label>Upload de Imagem</label>
<input id="uploadImage" type="file" accept="image/*">
</div>

</div>

<div class="actions">

<button onclick="generateImage()">Gerar Imagem</button>

<button onclick="downloadImage()">
Salvar PNG
</button>

</div>

<div class="canvas-area">

<canvas id="canvas"></canvas>

</div>

</div>

<script>

const canvas = document.getElementById("canvas");
const ctx = canvas.getContext("2d");

let uploadedImage = null;

document
.getElementById("uploadImage")
.addEventListener("change", function(e){

const file = e.target.files[0];

if(!file) return;

const img = new Image();

img.onload = ()=>{

uploadedImage = img;

generateImage();

};

img.src = URL.createObjectURL(file);

});

function generateImage(){

const text =
document
.getElementById("textInput")
.value
.trim();

const size =
parseInt(
document
.getElementById("sizeInput")
.value
) || 256;

const bgColor =
"#"+
document
.getElementById("bgInput")
.value
.replace("#","");

const textColor =
"#"+
document
.getElementById("textColorInput")
.value
.replace("#","");

canvas.width = size;
canvas.height = size;

ctx.clearRect(0,0,size,size);

ctx.fillStyle = bgColor;
ctx.fillRect(0,0,size,size);

if(uploadedImage){

const shortest =
Math.min(
uploadedImage.width,
uploadedImage.height
);

const sx =
(uploadedImage.width-shortest)/2;

const sy =
(uploadedImage.height-shortest)/2;

ctx.drawImage(
uploadedImage,
sx,
sy,
shortest,
shortest,
0,
0,
size,
size
);

}

if(text){

let fontSize = size;

ctx.font =
`bold ${fontSize}px Arial`;

while(
ctx.measureText(text).width >
(size*0.8)
){

fontSize -= 2;

ctx.font =
`bold ${fontSize}px Arial`;

}

ctx.fillStyle = textColor;

ctx.textAlign="center";

ctx.textBaseline="middle";

ctx.fillText(
text,
size/2,
size/2
);

}

}

function downloadImage(){

const fileName =
document
.getElementById("fileNameInput")
.value
.trim() || "imagem";

const link =
document.createElement("a");

link.download =
fileName + ".png";

link.href =
canvas.toDataURL("image/png");

link.click();

}

generateImage();

</script>

</body>
</html>
