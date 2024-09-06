# js-maria/nose.html in main
let xBolinha = 300;
let yBolinha = 200;
let diametro = 30; // Aumente o tamanho da bolinha
let velocidadeXBolinha = 2; // Diminua a velocidade

function setup() {
    createCanvas(600, 400);
}

function draw() {
    background(0, 0, 0); // Cor de fundo em RGB
    circle(xBolinha, yBolinha, diametro);
    xBolinha = xBolinha + velocidadeXBolinha;

    if (xBolinha + raio > width || xBolinha - raio < 0) {
        velocidadeXBolinha = velocidadeXBolinha * -1;
    }
}



// Variáveis da raquete
let xRaquete = 5;
let yRaquete = 150;
let raqueteComprimento = 10;
let raqueteAltura = 90;

function mostraRaquete() {
    rect(xRaquete, yRaquete, raqueteComprimento, raqueteAltura);
}
