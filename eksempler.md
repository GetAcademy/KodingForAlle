## Forord
## Innhold
## 1 - HTML
Eksempel 1 i kapittel 1 - HTML
```html
<h1>Min første web-side</h1>
```
Eksempel 2 i kapittel 1 - HTML
```html
<!DOCTYPE html>
<html>
<head>
    <title>Arkfaneoverskrift</title>
</head>
<body>
    <h1>Overskriften</h1>
    <p>Dette er et avsnitt.</p>
    <p>Dette er et avsnitt.</p>
</body>
</html>
```
Eksempel 3 i kapittel 1 - HTML
```html
☰ Vinlotterix<br/>
<input type="checkbox"/> Personer + ✎<br/>
<input type="checkbox" checked/> Per &nbsp;&nbsp;&nbsp;&nbsp;☒<br/>
<input type="checkbox" checked/> Pål &nbsp;&nbsp;&nbsp;&nbsp;☒<br/>
<input type="checkbox" /> Espen ☒<br/>
<input type="checkbox" checked/> Ole &nbsp;&nbsp;&nbsp;&nbsp;☒<br/>
<button>Trekk!</button> <input type="text" size="1" value="1"/>
<button>▲</button>
<button>▼</button>
```
Eksempel 4 i kapittel 1 - HTML
```html
☰ Vinlotterix<br/>
<small>onsdag 17.10.18</small><br/>
<b>Vinneren er Ole!</b><br/>
<small>Trukket fra totalt 3 personer: Per, Pål og Ole</small>
```
Eksempel 5 i kapittel 1 - HTML
```html
<table><tr><td>
<button>Personer</button><br/>
<button>Vinnere</button><br/>
<button>Om</button><br/>
<button>Exit</button><br/>
</td><td>
☰ Vinlotte<br/>
<small>onsdag 17.10</small><br/>
<b>Vinneren </b><br/>
<small>Trukket fra </small>
</td></tr></table>
```
## 2 - CSS
Eksempel 1 i kapittel 2 - CSS
```html
<!DOCTYPE html>
<html>
<head>
    <title>Arkfaneoverskrift</title>
    <style>
        h1 {
            color: blue;
        }
        p {
            color: green;
        }
    </style>
</head>
<body>
    <h1>Overskriften</h1>
    <p>
        Dette er et avsnitt 1. Dette er 
        et avsnitt . Dette er et avsnitt 1. 
        Dette er et avsnitt 1. Dette er 
        et avsnitt 1. Dette er et avsnitt 1.
        Dette er et avsnitt 1. Dette er 
        et avsnitt 1.
    </p>
    <p>
        Dette er et avsnitt 2. Dette er 
        et avsnitt 2. Dette er et avsnitt 2. 
        Dette er et avsnitt 2. Dette er 
        et avsnitt 2. Dette er et avsnitt 2.
        Dette er et avsnitt 2. Dette er 
        et avsnitt 2.
    </p>
</body>
</html>
```
Eksempel 2 i kapittel 2 - CSS
```html
<head>
    <title>Arkfaneoverskrift</title>
    <style>
        h1 {
            color: white;
            background-color: blue;            
        }

        div {
            color: green;
            background-color: lightgray;
            padding: 20px;
            margin: 40px;
            border: darkblue 1px solid;
            height: 70px;
            width: 50px;
        }
    </style>
</head>
<body>
    <h1>Overskriften</h1>
    <div>A</div>
    <div>B</div>
    <div>C</div>
</body>
```
Eksempel 3 i kapittel 2 - CSS
```html
<div>A</div>
<div class="specialEffect">B</div>
<div>C</div>
```
Eksempel 4 i kapittel 2 - CSS
```html
<div class="specialEffect">B</div>
``` 
## Vinlotterix - Prototyping 2 - CSS
Eksempel 1 i kapittel Vinlotterix - Prototyping 2 - CSS
```html
<div class="screen">
    <span>☰ Vinlotterix 🍷</span><br />
    <input type="checkbox" /> Personer + ✎<br />
    <input type="checkbox" checked /> Per &nbsp;&nbsp;&nbsp;&nbsp;☒<br />
    <input type="checkbox" checked /> Pål &nbsp;&nbsp;&nbsp;&nbsp;☒<br />
    <input type="checkbox" /> Espen ☒<br />
    <input type="checkbox" checked /> Ole &nbsp;&nbsp;&nbsp;&nbsp;☒<br />
    <button>Trekk!</button> <input type="text" size="1" value="1" />
    <button>▲</button>
    <button>▼</button>
</div>

<div class="screen">
    <span>☰ Vinlotterix 🍷</span><br />
    <small>onsdag 17.10.18</small><br />
    <b>Vinneren er Ole!</b><br />
    <small>Trukket fra totalt 3 personer: Per, Pål og Ole</small>
</div>

<div class="screen">
    <div class="menu">
        <button class="fixed">Personer</button><br />
        <button class="fixed">Vinnere</button><br />
        <button class="fixed">Om</button><br />
        <button class="fixed">Exit</button><br />
    </div>
    <div>
        <span>☰ Vinlotteri</span><br />
        <small>onsdag 17.10.18</small><br />
        <b>Vinneren er</b><br />
        <small>
            Trukket fra total<br />
            Per, Pål og Ole
        </small>
    </div>
</div>
```
Eksempel 2 i kapittel Vinlotterix - Prototyping 2 - CSS
```css
div.menu {
    float: left;
    height: 100%;
    padding-right: 4px;
}

div.screen {
    border: 1px solid gray;
    float: left;
    height: 200px;
    width: 170px;
    margin-left: 20px;
    background-color: rgb(250, 250, 250);
    color: black;
    padding: 0px 4px;
}

span {
    color: rgb(137,24,38);
    font-weight: bolder;
}

button {
    background-color: rgb(137,24,38);
    color: rgb(250, 250, 250);
}

    button.fixed {
        width: 70px;
        margin: 2px 4px;
    }
```
## CSS - fullskjermslayout ved hjelp av CSS Grid
Eksempel 1 i kapittel CSS - fullskjermslayout ved hjelp av CSS Grid
```html
<body>
    <div class="page"        style="background-color: lightblue">
        <div class="header"  style="background-color: lightcoral">Header</div>
        <div class="meny"    style="background-color: lightseagreen">Meny</div>
        <div class="innhold" style="background-color: lightgray">Innhold</div>
        <div class="footer"  style="background-color: blanchedalmond">Footer</div>
    </div>
</body>
```
Eksempel 2 i kapittel CSS - fullskjermslayout ved hjelp av CSS Grid
```html
<div class="page" style="display: grid; background-color: lightblue">
```
Eksempel 3 i kapittel CSS - fullskjermslayout ved hjelp av CSS Grid
```css
div.page {
    display: grid;
}
```
Eksempel 4 i kapittel CSS - fullskjermslayout ved hjelp av CSS Grid
```css
div.page {
    height: 100vh;
    display: grid;
    grid-template-columns: 2fr 1fr 3fr;
}
```
Eksempel 5 i kapittel CSS - fullskjermslayout ved hjelp av CSS Grid
```css
div.page {
    display: grid;
    height: 100vh;
    grid-template-columns: 1fr 2fr;
    grid-template-rows: 1fr 8fr 1fr;
    grid-template-areas: 'meny header' 
                         'meny innhold' 
                         'footer footer';
}

div.header {
    grid-area: header;
}

div.meny {
    grid-area: meny;
}

div.innhold {
    grid-area: innhold;
}

div.footer {
    grid-area: footer;
}
```
## Vinlotterix - prototyping 3 - CSS Grid
Eksempel 1 i kapittel Vinlotterix - prototyping 3 - CSS Grid
```css
div.page {
    display: grid;
    height: 100vh;
    grid-template-columns: 200px 2fr;
    grid-template-rows: 40px 1fr;
    grid-template-areas: 'meny header' 
                         'meny innhold';
}
```
Eksempel 2 i kapittel Vinlotterix - prototyping 3 - CSS Grid
```css
    grid-template-areas: 'header header' 
                         'innhold innhold';
```
Eksempel 3 i kapittel Vinlotterix - prototyping 3 - CSS Grid
```css
div.page {
    display: grid;
    height: 100vh;
    grid-template-columns: 1fr;
    grid-template-rows: 40px 1fr;
    grid-template-areas: 'header' 
                         'innhold';
}
```
## Responsivt webdesign
Eksempel 1 i kapittel Responsivt webdesign
```css
@media only screen and (max-width: 600px) {
    div.page {
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr 5fr 1fr;
        grid-template-areas: 'header' 
                             'meny'
                             'innhold'
                             'footer';
    }
}
```
## 3 - Å publisere det man har laget
Eksempel 1 i kapittel 3 - Å publisere det man har laget
```html
<!DOCTYPE html>
<html>
<head>
    <title>Terjes snasne side</title>
    <style>
        div, body {
            padding: 10vh 10vw;
            margin: 0;
            color: darkgreen;
            border-radius: 50%;
        }
    </style>
</head>
<body style="background-color: red">
    <div style="background-color: orange">
        <div style="background-color: yellow; height: 30vh">
            <h1>Velkommen til Terjes snasne side</h1>
        </div>
    </div>
</body>
</html>
```
## 4 - Grunnferdigheter i Javascript
Eksempel 1 i kapittel 4 - Grunnferdigheter i Javascript
```html
<script>
    alert('Hei på deg!');
</script>
```
Eksempel 2 i kapittel 4 - Grunnferdigheter i Javascript
```html
<h1 onclick="alert('Takk :-)');">Trykk på meg!</h1>
``` 
Eksempel 3 i kapittel 4 - Grunnferdigheter i Javascript
```js
alert('Hei');
alert('på');
alert('deg!');
```
Eksempel 4 i kapittel 4 - Grunnferdigheter i Javascript
```js
function heiPåDeg() {
    alert('Hei');
    alert('på');
    alert('deg!');
}
```
Eksempel 5 i kapittel 4 - Grunnferdigheter i Javascript
```html
<h1 id="overskrift" onclick="endreTekst()">Trykk på meg!</h1>
<script>
    function endreTekst() {
        document.getElementById('overskrift').innerHTML = 'Takk :-)';
    }
</script>
```
Eksempel 6 i kapittel 4 - Grunnferdigheter i Javascript
```html
<h1 onclick="endreTekst()">Trykk på meg for å endre overskriften under!</h1>
<h1 id="overskrift" >Trykk på overskriften over for å endre meg!</h1>
<script>
    function endreTekst() {
        document.getElementById('overskrift').innerHTML = 'Takk :-)';
    }
</script>
```
Eksempel 7 i kapittel 4 - Grunnferdigheter i Javascript
```html
<b id="overskrift" onclick="endreTekst()">Trykk for prikker:</b>
<script>
    function endreTekst() {
        document.getElementById('overskrift').innerHTML += ' •';
    }
</script>
```
Eksempel 8 i kapittel 4 - Grunnferdigheter i Javascript
```html
<div id="minDiv" style="background-color: red;">Hei</div>
```
Eksempel 9 i kapittel 4 - Grunnferdigheter i Javascript
```js
document.getElementById('minDiv').style.backgroundColor = 'red';
```
Eksempel 10 i kapittel 4 - Grunnferdigheter i Javascript
```css
div.rødOgFin {
    background-color: red;
}
```
Eksempel 11 i kapittel 4 - Grunnferdigheter i Javascript
```js
document.getElementById('minDiv').classList.add('rødOgFin');
```
Eksempel 12 i kapittel 4 - Grunnferdigheter i Javascript
```js
document.getElementById('minDiv').classList.remove('rødOgFin');
```
Eksempel 13 i kapittel 4 - Grunnferdigheter i Javascript
```html
<div id="innhold">
    Jeg tenker på et tall mellom 1 og 20. Tipp hvilket!<br />
    <input type="text" /> <button onclick="tipp1()">Tipp</button>
</div>
```
Eksempel 14 i kapittel 4 - Grunnferdigheter i Javascript
```js
function tipp1() {
    document.getElementById('innhold').innerHTML = `
            Du tippet 27. Det er for høyt - tipp igjen!<br/>
            <input type="text"/><button onclick="tipp2()">Tipp</button>
            `;
}
```
Eksempel 15 i kapittel 4 - Grunnferdigheter i Javascript
```js
function tipp2() {
    document.getElementById('innhold').innerHTML = `
            Du tippet 12 - og det er riktig! 😀<br/>
            <button onclick="tipp2()">Start på nytt</button>
            `;
}
```
Eksempel 16 i kapittel 4 - Grunnferdigheter i Javascript
```html
<div class="page" id="page">
    <div class="header" id="header">
        <button onclick="visOgSkjulMeny()">☰</button> 
        Vinlotterix 🍷
    </div>
    <div class="innhold" id="innhold"></div>
    <div class="meny" id="meny">
        <button class="fixed" onclick="visPersoner()">Personer</button><br />
        <button class="fixed" onclick="visVinnere1()">Vinnere</button><br />
        <button class="fixed">Om</button><br />
        <button class="fixed">Exit</button><br />
    </div>
</div>
```
Eksempel 17 i kapittel 4 - Grunnferdigheter i Javascript
```js
function visOgSkjulMeny() {
    document.getElementById('page').classList.toggle('pageUtenMeny');
}
```
Eksempel 18 i kapittel 4 - Grunnferdigheter i Javascript
```css
div.pageUtenMeny {
    grid-template-columns: 0px 2fr;
}
```
Eksempel 19 i kapittel 4 - Grunnferdigheter i Javascript
```js
function visPersoner() {
    document.getElementById('innhold').innerHTML = `
                <table>
                    <tr><td><input type="checkbox"/></td><td>Personer</td><td>+</td><td>✎</td></tr>
                    <tr><td><input type="checkbox" checked/></td><td>Per</td><td onclick="visPersonerMinusPer()">☒</td></tr>
                    <tr><td><input type="checkbox" checked/></td><td>Pål</td><td>☒</td></tr>
                    <tr><td><input type="checkbox"/></td><td>Espen</td><td>☒</td></tr>
                    <tr><td><input type="checkbox" checked/></td><td>Ole</td><td>☒</td></tr>
                    <tr><td colspan="4"><button onclick="visVinnere2()">Trekk!</button> <input type="text" size="1" value="1"/>
                        <button>▲</button>
                        <button>▼</button></td></tr>
                </table>
                `;
}

function visVinnere1() {
    document.getElementById('innhold').innerHTML = `
        <p>
            <small>onsdag 17.10.18</small><br/>
            <b>Vinneren er Ole!</b><br/>
            <small>Trukket fra totalt 3 personer: Per, Pål og Ole</small>
        </p>
        `;
}
```
Eksempel 20 i kapittel 4 - Grunnferdigheter i Javascript
```html
<button onclick="alert(this.innerHTML)">Hei!</button>
<button onclick="alert(this.innerHTML)">Hallo!</button>
```
Eksempel 21 i kapittel 4 - Grunnferdigheter i Javascript
```html
<button onclick="this.innerHTML = 'x'">Hei!</button>
<button onclick="this.innerHTML = 'x'">Hallo!</button>
```
Eksempel 22 i kapittel 4 - Grunnferdigheter i Javascript
```html
<h1 onclick="trykk()">Trykk!</h1>
<h1 id="o">Trykk!</h1>
<script>
    function trykk() {
        document.getElementById('o').innerHTML = 'x';
    }
</script>
```

Eksempel 23 i kapittel 4 - Grunnferdigheter i Javascript
```html
<h1 onclick="trykk(this)">Trykk!</h1>
<h1 onclick="trykk(this)">Trykk!</h1>
<script>
    function trykk(trykketPåTag) {
        trykketPåTag.innerHTML = 'x';
    }
</script>
```
Eksempel 24 i kapittel 4 - Grunnferdigheter i Javascript
```js
alert('Hei' + 'på' + 'deg!');
```
Eksempel 25 i kapittel 4 - Grunnferdigheter i Javascript
```html
<button onclick="alert('Hei, ' + this.innerHTML + '!')">Per</button>
<button onclick="alert('Hei, ' + this.innerHTML + '!')">Pål</button>
<button onclick="alert('Hei, ' + this.innerHTML + '!')">Espen</button>
```
Eksempel 26 i kapittel 4 - Grunnferdigheter i Javascript
```js
var tekst = 'Hei, ' + navn + '. Hvordan står det til i ' + sted + '?';
```
Eksempel 27 i kapittel 4 - Grunnferdigheter i Javascript
```js
var tekst = `Hei, ${navn}. Hvordan står det til i ${sted}?`;
```
Eksempel 28 i kapittel 4 - Grunnferdigheter i Javascript
```js
var tekst = `Hei, ${navn}. 
             Hvordan står det til i ${sted}?`;
```
Eksempel 29 i kapittel 4 - Grunnferdigheter i Javascript
```js
var tekst = 'Hei, ' + navn + '.' 
          + 'Hvordan står det til i ' + sted + '?';
```
Eksempel 30 i kapittel 4 - Grunnferdigheter i Javascript
```html
<script>
    console.log('Hei');
    console.log('på');
    console.log('deg!');
</script>
```
Eksempel 31 i kapittel 4 - Grunnferdigheter i Javascript
```js
var navnFraSkjema = document.getElementById('navn').value;
```
Eksempel 32 i kapittel 4 - Grunnferdigheter i Javascript
```js
var minDiv = document.getElementById('minDiv');
minDiv.style.backgroundColor = '#4567ab';
minDiv.style.color = '#4567ab';
minDiv.style.padding = '4px';
minDiv.classList.add('active');
minDiv.classList.remove('old');
minDiv.classList.toggle('something');
```
Eksempel 33 i kapittel 4 - Grunnferdigheter i Javascript
```html
<div class="something old"></div>
```
Eksempel 34 i kapittel 4 - Grunnferdigheter i Javascript
```html
<div class="active"></div>
```
Eksempel 35 i kapittel 4 - Grunnferdigheter i Javascript
```html
<input type="text"
       onclick="console.log('onclick ' + this.value)"
       oninput="console.log('oninput ' + this.value)"
       onchange="console.log('onchange ' + this.value)"/>
```
Eksempel 36 i kapittel 4 - Grunnferdigheter i Javascript
```
onclick 
oninput h
oninput he
oninput hei
onchange hei
```
## 5 - Variabler
Eksempel 1 i kapittel 5 - Variabler
```js
var teller;
```
Eksempel 2 i kapittel 5 - Variabler
```js
teller = 0;
```
Eksempel 3 i kapittel 5 - Variabler
```js
var tall = 123;
```
Eksempel 4 i kapittel 5 - Variabler
```js
a = 5;
b = a;
```
Eksempel 5 i kapittel 5 - Variabler
```js
a = 5;
b = a;
a = 6;
a = 7;
a = 8;
```
Eksempel 6 i kapittel 5 - Variabler
```js
var navn = 'Terje';
```
Eksempel 7 i kapittel 5 - Variabler
```js
var navn = Terje;
```
Eksempel 8 i kapittel 5 - Variabler
```js
var tekst = 'Hei' + ' på ' + 'deg!';
console.log(tekst);
```
Eksempel 9 i kapittel 5 - Variabler
```js
var divHtml = document.getElementById('div5').innerHTML;
```
Eksempel 10 i kapittel 5 - Variabler
```js
document.getElementById('mainContent').innerHTML = 'B!';
``` 
Eksempel 11 i kapittel 5 - Variabler
```js
var mainContentDiv = document.getElementById('mainContent');
mainContentDiv.innerHTML = 'B!';
``` 
Eksempel 12 i kapittel 5 - Variabler
```js
var contentTmp = document.getElementById('divA').innerHTML;
document.getElementById('divA').innerHTML = 
    document.getElementById('divB').innerHTML;
document.getElementById('divB').innerHTML = contentTmp;
```
Eksempel 13 i kapittel 5 - Variabler
```js
var divA = document.getElementById('divA');
var divB = document.getElementById('divB');
var contentTmp = divA.innerHTML;
divA.innerHTML = divB.innerHTML;
divB.innerHTML = contentTmp;
```
Eksempel 14 i kapittel 5 - Variabler
```html
<div id="content">Hallo!</div>
<button onclick="wrap()">Wrap!</button>
<script>
    function wrap() {
        var contentDiv = document.getElementById('content');
        var innhold = contentDiv.innerHTML;
        contentDiv.innerHTML = '<ul><li>' + innhold + '</li><li>'
            + innhold + '</li></ul>';
    }
</script>
```
Eksempel 15 i kapittel 5 - Variabler
```js
function wrap() {
    var contentDiv = document.getElementById('content');
    var innhold = contentDiv.innerHTML;
    contentDiv.innerHTML = `
        <ul>
            <li>${innhold}</li>
            <li>${innhold}</li>
        </ul>`;
}
```
Eksempel 16 i kapittel 5 - Variabler
```js
var antallKlikk = 0;

function tell() {
    antallKlikk++;
    console.log(antallKlikk);
}
```
Eksempel 17 i kapittel 5 - Variabler
```html
<button onclick="merk(this)">A</button>
<button onclick="merk(this)">B</button>
<button onclick="merk(this)">C</button>
```
Eksempel 18 i kapittel 5 - Variabler
```js
function merk(element){
  element.style.border = 'dashed orange 2px';
}
```
Eksempel 19 i kapittel 5 - Variabler
```js
var forrigeElement;

function merk(element){
  element.style.border = 'dashed orange 2px';
  forrigeElement.style.border = 'none';
  forrigeElement = element;
}
```
Eksempel 20 i kapittel 5 - Variabler
```html
<button id="knappA" onclick="merk(this)">A</button>
<button onclick="merk(this)">B</button>
<button onclick="merk(this)">C</button>
<script>
    var forrigeElement = document.getElementById('knappA');

    function merk(element){
    element.style.border = 'dashed orange 2px';
    forrigeElement.style.border = 'none';
    forrigeElement = element;
    }
</script>
```
Eksempel 21 i kapittel 5 - Variabler
```js
var tekstA = '5';
var tekstB = '7';
var tallA = parseInt(tekstA);
var tallB = parseInt(tekstB);
var x = tallA + tallB; 
```
Eksempel 22 i kapittel 5 - Variabler
```html
<input id="tallA" type="range" min="1" max="100" step="1" value="2" 
       oninput="calculate()" />
<input id="tallB" type="range" min="1" max="100" step="1" value="2" 
       oninput="calculate()" />
<div id="resultat"></div>
<script>
    var resultatDiv = document.getElementById('resultat');
    var tallAInput = document.getElementById('tallA');
    var tallBInput = document.getElementById('tallB');
    calculate();
    function calculate() {
        var tallA = parseInt(tallAInput.value);
        var tallB = parseInt(tallBInput.value);
        var sum = tallA + tallB;
        var differense = tallA - tallB;
        var produkt = tallA * tallB;
        var kvotient = tallA / tallB;
        resultatDiv.innerHTML = '' +
            tallA + '+' + tallB + '=' + sum + '<br/>' +
            tallA + '-' + tallB + '=' + differense + '<br/>' +
            tallA + '*' + tallB + '=' + produkt + '<br/>' +
            tallA + '/' + tallB + '=' + kvotient;
    }
</script>
```
Eksempel 23 i kapittel 5 - Variabler
```js
var resultatDiv = document.getElementById('resultat');
calculate();
function calculate() {
    var tallA = 100 + Math.floor(Math.random() * 10);
    var tallB = 100 + Math.floor(Math.random() * 10);
    var sum = tallA + tallB;
    var differense = tallA - tallB;
    var produkt = tallA * tallB;
    var kvotient = tallA / tallB;
    resultatDiv.innerHTML = '' +
        tallA + '+' + tallB + '=' + sum + '<br/>' +
        tallA + '-' + tallB + '=' + differense + '<br/>' +
        tallA + '*' + tallB + '=' + produkt + '<br/>' +
        tallA + '/' + tallB + '=' + kvotient;
}
```
## 6 - Valgsetninger
Eksempel 1 i kapittel 6 - Valgsetninger
```html
<button onclick="tell()">Tell</button>
<div id="info"></div>
<script>
var antallKlikk = 0;
var infoDiv = document.getElementById('info');

function tell() {
    antallKlikk++;
    infoDiv.innerHTML = 'Du har klikket ' + antallKlikk + ' ganger.';
}
</script>
```
Eksempel 2 i kapittel 6 - Valgsetninger
```js
antallKlikk++;
if( antallKlikk == 10 ) {
    infoDiv.innerHTML = 'Du har klikket 10 ganger.';
}
```
Eksempel 3 i kapittel 6 - Valgsetninger
```js
antallKlikk++;
if( antallKlikk == 10 ) {
    infoDiv.innerHTML = 'Du har klikket 10 ganger.';
} else {
    infoDiv.innerHTML = '';
}
```
Eksempel 4 i kapittel 6 - Valgsetninger
```js
antallKlikk++;
infoDiv.innerHTML = '';
if( antallKlikk == 10 ) {
    infoDiv.innerHTML = 'Du har klikket 10 ganger.';
}
```
Eksempel 5 i kapittel 6 - Valgsetninger
```js
antallKlikk++;
if( antallKlikk < 10 ) {
    infoDiv.innerHTML = 'Du har klikket 9 ganger eller mindre.';
} else {
    infoDiv.innerHTML = 'Du har klikket 10 ganger eller mer.';
}
```
Eksempel 6 i kapittel 6 - Valgsetninger
```js
antallKlikk++;
if( antallKlikk >= 10 ) {
    infoDiv.innerHTML = 'Du har klikket 10 ganger eller mer.';
} else {
    infoDiv.innerHTML = 'Du har klikket 9 ganger eller mindre.';
}
```
Eksempel 7 i kapittel 6 - Valgsetninger
```js
var månedsnavn;
if (måned == 1) {
    månedsnavn = 'Januar';
} else if (måned == 2) {
    månedsnavn = 'Februar';
} else if (måned == 3) {
    månedsnavn = 'Mars';
} else if (måned == 4) {
    månedsnavn = 'April';
} else if (måned == 5) {
    månedsnavn = 'Mai';
} else if (måned == 6) {
    månedsnavn = 'Juni';
} else if (måned == 7) {
    månedsnavn = 'Juli';
} else if (måned == 8) {
    månedsnavn = 'August';
} else if (måned == 9) {
    månedsnavn = 'September';
} else if (måned == 10) {
    månedsnavn = 'Oktober';
} else if (måned == 11) {
    månedsnavn = 'November';
} else if (måned == 12) {
    månedsnavn = 'Desember';
} else {
    månedsnavn = '<ukjent månedsnummer ' + måned + '>';
}
```
Eksempel 8 i kapittel 6 - Valgsetninger
```js
if (måned == 1) månedsnavn = 'Januar';
else if (måned == 2) månedsnavn = 'Februar';
else if (måned == 3) månedsnavn = 'Mars';
else if (måned == 4) månedsnavn = 'April';
else if (måned == 5) månedsnavn = 'Mai';
else if (måned == 6) månedsnavn = 'Juni';
else if (måned == 7) månedsnavn = 'Juli';
else if (måned == 8) månedsnavn = 'August';
else if (måned == 9) månedsnavn = 'September';
else if (måned == 10) månedsnavn = 'Oktober';
else if (måned == 11) månedsnavn = 'November';
else if (måned == 12) månedsnavn = 'Desember';
else månedsnavn = '<ukjent månedsnummer ' + måned + '>';
```
Eksempel 9 i kapittel 6 - Valgsetninger
```js
if(a == 1) x = 10;
else x = 20;
     y = 5;
```
Eksempel 10 i kapittel 6 - Valgsetninger
```js
if(a == 1) {
    x = 10;
} else {
    x = 20;
    y = 5;
}
```
Eksempel 11 i kapittel 6 - Valgsetninger
```js
if( navn == 'Terje' ) {
    alert('Terje, jo!');
}
```
Eksempel 12 i kapittel 6 - Valgsetninger
```html
<div id="info"></div>
<p>Endre på tekstene! (Prøv også å fylle ut tall: 11, 101, 102)</p>
<input type="text" id="txt1" oninput="findFirst()" value="Per" /><br />
<input type="text" id="txt2" oninput="findFirst()" value="Pål" /><br />
<input type="text" id="txt3" oninput="findFirst()" value="Espen" /><br />
<script>
    var infoDiv = document.getElementById('info');
    var txtDiv1 = document.getElementById('txt1');
    var txtDiv2 = document.getElementById('txt2');
    var txtDiv3 = document.getElementById('txt3');
    findFirst();

    function findFirst() {
        var txt1 = txtDiv1.value;
        var txt2 = txtDiv2.value;
        var txt3 = txtDiv3.value;
        var html = '';

        if (txt1 == txt2) html += 'Tekst 1 og 2 er like<br/>';
        if (txt1 != txt2) html += '<del>Tekst 1 og 2 er like</del><br/>';

        if (txt1 == txt3) html += 'Tekst 1 og 3 er like<br/>';
        if (txt1 != txt3) html += '<del>Tekst 1 og 3 er like</del><br/>';

        if (txt3 == txt2) html += 'Tekst 2 og 3 er like<br/>';
        if (txt3 != txt2) html += '<del>Tekst 2 og 3 er like</del><br/>';

        html += 'Om vi sorterer de tre tekstene, er denne den første:<br/>';
        if (txt1 <= txt2) {
            if (txt3 <= txt1) infoDiv.innerHTML += txt3;
            else html += txt1;
        } else {
            if (txt3 <= txt2) infoDiv.innerHTML += txt3;
            else html += txt2;
        }
        infoDiv.innerHTML = html;
    }
</script>
```
Eksempel 13 i kapittel 6 - Valgsetninger
```js
if (txt1 == txt2) html += 'Tekst 1 og 2 er like<br/>';
if (txt1 != txt2) html += '<del>Tekst 1 og 2 er like</del><br/>';
```
Eksempel 14 i kapittel 6 - Valgsetninger
```js
if (txt1 == txt2) html += 'Tekst 1 og 2 er like<br/>';
else html += '<del>Tekst 1 og 2 er like</del><br/>';
```
Eksempel 15 i kapittel 6 - Valgsetninger
```js
document.getElementById('abc').innerHTML = '<h1>Overskrift</h1>';
```
Eksempel 16 i kapittel 6 - Valgsetninger
```js
var abcDiv = document.getElementById('abc');
abcDiv.innerHTML = '<h1>Overskrift</h1>';
```
Eksempel 17 i kapittel 6 - Valgsetninger
```js
var div1 = document.getElementById('aaa');
var div2 = document.getElementById('bbb');
if( div1 == div2 ) {
    ...
}
```
Eksempel 18 i kapittel 6 - Valgsetninger
```js
var div1 = document.getElementById('aaa');
var div2 = document.getElementById('aaa');
if( div1 == div2 ) {
    ...
}
```
Eksempel 19 i kapittel 6 - Valgsetninger
```html
<div id="a" onclick="velg(this)">A</div>
<div id="b" onclick="velg(this)">B</div>
<div id="c" onclick="velg(this)">C</div>
<div id="info">Trykk på en firkant!</div>

<script>
    var infoDiv = document.getElementById('info');
    var divA = document.getElementById('a');
    var divB = document.getElementById('b');
    var divC = document.getElementById('c');
    var forrigeKnapp;

    function doClick(valgtKnappNå) {
        if (valgtKnappNå == divA) infoDiv.innerHTML = 'Du valgte A. ';
        else if (valgtKnappNå == divB) infoDiv.innerHTML = 'Du valgte B. ';
        else if (valgtKnappNå == divC) infoDiv.innerHTML = 'Du valgte C. ';

        if (valgtKnappNå == forrigeKnapp) {
            infoDiv.innerHTML += 'Du valgte samme som sist!';
        }

        forrigeKnapp = valgtKnappNå;
    }
</script>
```
Eksempel 20 i kapittel 6 - Valgsetninger
```js
if (txt1 <= txt2) {
    if (txt3 <= txt1) html += txt3;
    else html += txt1;
} else {
    if (txt3 <= txt2) html += txt3;
    else html += txt2;
}
```
Eksempel 21 i kapittel 6 - Valgsetninger
```js
if( betingelse1 ) {
    if( betingelse2 ) {
        ...
    }
}
```
Eksempel 22 i kapittel 6 - Valgsetninger
```js
if( betingelse1 & betingelse2 ) {
    ...
}
```
Eksempel 23 i kapittel 6 - Valgsetninger
```js
if (txt1 <= txt2 & txt1 <= txt3) html += txt1;
else if (txt2 <= txt1 & txt2 <= txt3) html += txt2;
else html += txt3;
```
Eksempel 24 i kapittel 6 - Valgsetninger
```js
if (txt1 <= txt2 & txt1 <= txt3) html += txt1;
else if (txt2 <= txt3) html += txt2;
else html += txt3;
```
Eksempel 25 i kapittel 6 - Valgsetninger
```js
if( txt != undefined & txt.length == 10 )
```  
Eksempel 26 i kapittel 6 - Valgsetninger
```js
if( txt != undefined && txt.length == 10 )
```  
Eksempel 27 i kapittel 6 - Valgsetninger
```js
alert( `Hei, ${ name || 'kompis' }!`); 
```
Eksempel 28 i kapittel 6 - Valgsetninger
```html
<br/>A <input type="checkbox"/>
<br/>B <input type="checkbox" checked="checked"/>
```
Eksempel 29 i kapittel 6 - Valgsetninger
```js
var erValgt = document.getElementById('chk1').checked;
```
Eksempel 30 i kapittel 6 - Valgsetninger
```html
<div id="info"></div>
<input id="a" type="checkbox" onchange="info()" />Checkbox A<br />
<input id="b" type="checkbox" onchange="info()" />Checkbox B<br />

<script>
    var infoDiv = document.getElementById('info');
    var chk1 = document.getElementById('a');
    var chk2 = document.getElementById('b');
    info();

    function info() {
        var erValgt1 = chk1.checked;
        var erValgt2 = chk2.checked;

        if ( erValgt1 && erValgt2 ) {
            infoDiv.innerHTML = 'Begge er valgt';
        } else if ( erValgt1 || erValgt2 ) {
            infoDiv.innerHTML = 'Én av dem er valgt';
        } else {
            infoDiv.innerHTML = 'Ingen er valgt';
        }
    }
</script>
```
Eksempel 31 i kapittel 6 - Valgsetninger
```js
var erValgt = document.getElementById('chk1').checked;
if( erValgt ) {
    ...
}
```
Eksempel 32 i kapittel 6 - Valgsetninger
```js
if( document.getElementById('chk1').checked ) {
    ...
}
```
Eksempel 33 i kapittel 6 - Valgsetninger
```js
if( n < 10 ) {
    ...
}
```
Eksempel 34 i kapittel 6 - Valgsetninger
```js
var verdienErRiktig = n < 10;
if( verdienErRiktig ) {
    ...
}
```
Eksempel 35 i kapittel 6 - Valgsetninger
```js
var a = true;
var b = false;
```
Eksempel 36 i kapittel 6 - Valgsetninger
```js
if( !document.getElementById('chk1').checked ) {
    ...
}
```
Eksempel 37 i kapittel 6 - Valgsetninger
```html
<h3>Pizza-bestilling</h3>
<div id="info" >Gjør ett valg på hver linje:</div>

Bunn: <input id="tykkBunn" type="radio" name="bunn" />Tykk
<input id="tynnBunn" type="radio" name="bunn" />Tynn <br />

Fyll: <input id="fyllTaco" type="radio" name="fyll" />Taco
<input id="fyllKylling" type="radio" name="fyll" />Kylling
<input id="fyllPepperoni" type="radio" name="fyll" />Pepperoni<br />

Størrelse: <input id="stor" type="radio" name="str" />Stor
<input id="middels" type="radio" name="str" />Middels
<input id="liten" type="radio" name="str"  />Liten<br />

<button id="bestill" onclick="bestill()">Bestill</button>
```
Eksempel 38 i kapittel 6 - Valgsetninger
```js
var btnBestill = document.getElementById('bestill');
var infoDiv = document.getElementById('info');
var bunnTykk = document.getElementById('tykkBunn');
var bunnTynn = document.getElementById('tynnBunn');
var fyllTaco = document.getElementById('fyllTaco');
var fyllKylling = document.getElementById('fyllKylling');
var fyllPepperoni = document.getElementById('fyllPepperoni');
var strStor = document.getElementById('stor');
var strMiddels = document.getElementById('middels');
var strLiten = document.getElementById('liten');
```
Eksempel 39 i kapittel 6 - Valgsetninger
```js
if ((bunnTykk.checked || bunnTynn.checked) &&
    (fyllTaco.checked || fyllKylling.checked || fyllPepperoni.checked) &&
    (strStor.checked || strMiddels.checked || strLiten.checked)) {
    infoDiv.innerHTML = 'Du har fylt ut alt og er klar til å bestille!';
} 
```
Eksempel 40 i kapittel 6 - Valgsetninger
```js
if ( bunnTykk.checked || bunnTynn.checked &&
     fyllTaco.checked || fyllKylling.checked || fyllPepperoni.checked &&
     strStor.checked || strMiddels.checked || strLiten.checked ) 
```
Eksempel 41 i kapittel 6 - Valgsetninger
```js
if ( bunnTykk.checked 
    || bunnTynn.checked && fyllTaco.checked 
    || fyllKylling.checked 
    || fyllPepperoni.checked && strStor.checked 
    || strMiddels.checked 
    || strLiten.checked ) 
```
Eksempel 42 i kapittel 6 - Valgsetninger
```js
else {
    infoDiv.innerHTML = 'Du har ikke valgt:';

    if (!bunnTykk.checked && !bunnTynn.checked) {
        infoDiv.innerHTML += '<li>bunn</li>';
    }
    if (!fyllTaco.checked && !fyllKylling.checked && !fyllPepperoni.checked) {
        infoDiv.innerHTML += '<li>fyll</li>';
    }
    if (!strStor.checked && !strMiddels.checked && !strLiten.checked) {
        infoDiv.innerHTML += '<li>størrelse</li>';
    }
}
```
## 7 - Funksjoner
Eksempel 1 i kapittel 7 - Funksjoner
```js
var popupDiv = document.getElementById('popup');

function visPopup() {
    popupDiv.innerHTML = 'Endringen er lagret. <br/><button onclick="lukkPopup()">Ok</button>';
}

function skulPopup() {
    popupDiv.innerHTML = '';
}
```
Eksempel 2 i kapittel 7 - Funksjoner
```js
function visPopup( tekst ) {
    popupDiv.innerHTML = tekst + '<br/><button onclick="lukkPopup()">Ok</button>';
}
```
Eksempel 3 i kapittel 7 - Funksjoner
```js
function visLagretPopup() {
    visPopup( 'Endringen er lagret.' );
}
```
Eksempel 4 i kapittel 7 - Funksjoner
```html
<button onclick="lukkPopup()">Ok</button>
```
Eksempel 5 i kapittel 7 - Funksjoner
```html
<button onclick="visPopup()">Ok</button>
```
Eksempel 6 i kapittel 7 - Funksjoner
```js
function visPopup( tekst ) {
    if( tekst ) {
        popupDiv.innerHTML = tekst + '<br/><button onclick="lukkPopup()">Ok</button>';
    } else {
        popupDiv.innerHTML = '';
    }
}
```
Eksempel 7 i kapittel 7 - Funksjoner
```js
function visPopup( tekst ) {
    popupDiv.innerHTML = tekst ? tekst + '<br/><button onclick="lukkPopup()">Ok</button>' : '';
}
```
Eksempel 8 i kapittel 7 - Funksjoner
```js
popupDiv.innerHTML = !tekst ? '' : tekst + '<br/><button onclick="lukkPopup()">Ok</button>';
```
Eksempel 9 i kapittel 7 - Funksjoner
```js
var tilfeldigTerningVerdi = Math.ceil( Math.random() * 6 );
```
Eksempel 10 i kapittel 7 - Funksjoner
```js
var tilfeldigTerningVerdi1 = Math.ceil( Math.random() * 6 );
var tilfeldigTerningVerdi2 = Math.ceil( Math.random() * 6 );
```
Eksempel 11 i kapittel 7 - Funksjoner
```js
function lagTilfeldigTerningverdi() {
    return Math.ceil( Math.random() * 6 ); 
}

var tilfeldigTerningVerdi1 = lagTilfeldigTerningverdi();
var tilfeldigTerningVerdi2 = lagTilfeldigTerningverdi();
```
Eksempel 12 i kapittel 7 - Funksjoner
```js
function bestill( antallBilletter ) {
    if( antallBilletter < 1 | antallBilletter > 6 ) return;
    // fortsett med å gjennomføre bestillingen her
}
```
Eksempel 13 i kapittel 7 - Funksjoner
```js
function tilfeldigTall(minimum, maksimum) {
    return minimum + Math.floor(Math.random() * (maksimum - minimum + 1));
}
```
Eksempel 14 i kapittel 7 - Funksjoner
```js
function tilfeldigTallEllerBokstavABCDEF() {
    var tall = tilfeldigTall(0, 15);
    if (tall < 10) return tall;
    else if( tall == 10) return 'a';
    else if( tall == 11) return 'b';
    else if( tall == 12) return 'c';
    else if( tall == 13) return 'd';
    else if( tall == 14) return 'e';
    else return 'f';
}
```
Eksempel 15 i kapittel 7 - Funksjoner
```js
function tilfeldigTallEllerBokstavABCDEF() {
    var tall = tilfeldigTall(0, 15);
    if (tall < 10) return tall;
    const charCodeA = 'a'.charCodeAt(0);
    return String.fromCharCode(tall - 10 + charCodeA);
}
```
Eksempel 16 i kapittel 7 - Funksjoner
```js
function tilfeldigFarge() {
    return '#' +
        tilfeldigTallEllerBokstavABCDEF() +
        tilfeldigTallEllerBokstavABCDEF() +
        tilfeldigTallEllerBokstavABCDEF() +
        tilfeldigTallEllerBokstavABCDEF() +
        tilfeldigTallEllerBokstavABCDEF() +
        tilfeldigTallEllerBokstavABCDEF();
}
```
Eksempel 17 i kapittel 7 - Funksjoner
```js
document.body.style.backgroundColor = tilfeldigFarge();
```
Eksempel 18 i kapittel 7 - Funksjoner
```html
<script>
    var a = 5;
</script>
```
Eksempel 19 i kapittel 7 - Funksjoner
```js
function telle() {
    var b = 5;
    b++;
    a++;
}
```
Eksempel 20 i kapittel 7 - Funksjoner
```js
const minDiv = document.getElementById('divenmin');
```
Eksempel 21 i kapittel 7 - Funksjoner
```html
<script>
    let a = 5; // a er tilgjengelig overalt

    function f() {
        let b = 6; // b er tilgjengelig i hele funksjonen f, men ingen andre steder
                   // Den "dør" når funksjonen er ferdig.
        if( a < 10 ) {
            let c = 7; // c er bare tilgjengelig i denne blokken, altså fra { på 
                       // forrige linje til } på neste linje
        } else {
            let c = 7; // Denne variabelen c er bare tilgjengelig i denne blokken, 
                       // altså fra { på forrige linje til } på neste linje
        }
    }
</script>
```
## 8 - Problemløsningsteknikker
Eksempel 1 i kapittel 8 - Problemløsningsteknikker
```js
function snu(tekst) {
    let snuddTekst = '';
    for (let i = tekst.length - 1; i >= 0; i--) {
        snuddTekst += tekst[i];
    }
    return snuddTekst;
}
```
Eksempel 2 i kapittel 8 - Problemløsningsteknikker
```js
function snu(tekst) {
    let snuddTekst = '';
    for (const bokstav of tekst) {
        snuddTekst = bokstav + snuddTekst;
    }
    return snuddTekst;
}
```
Eksempel 3 i kapittel 8 - Problemløsningsteknikker
```js
function sjekkAlleMuligheter() {
  return sjekkEnMulighet(1)
    || sjekkEnMulighet(2)
    || sjekkEnMulighet(3)
    || sjekkEnMulighet(4)
    || sjekkEnMulighet(5)
    || sjekkEnMulighet(6)
    || sjekkEnMulighet(7)
    || sjekkEnMulighet(8);
}

function sjekkEnMulighet() {
  return true eller false;
}
```
Eksempel 4 i kapittel 8 - Problemløsningsteknikker
```js
function sjekkAlleMuligheter() {
  return sjekkEnMulighet(0, 1, 2)  // rad 1
    || sjekkEnMulighet(3, 4, 5)  // rad 2
    || sjekkEnMulighet(6, 7, 8)  // rad 3
    || sjekkEnMulighet(0, 3, 6)  // kolonne 1
    || sjekkEnMulighet(1, 4, 7)  // kolonne 2
    || sjekkEnMulighet(2, 5, 8)  // kolonne 3
    || sjekkEnMulighet(0, 4, 8)  // diagonal 1
    || sjekkEnMulighet(2, 4, 6); // diagonal 2
}

function sjekkEnMulighet(indeks1, indeks2, indeks3) {
  return (model.ruter[indeks1] == 'x' || model.ruter[indeks1] == 'o')
    && model.ruter[indeks1] == model.ruter[indeks2]
    && model.ruter[indeks1] == model.ruter[indeks3];
}
```
Eksempel 5 i kapittel 8 - Problemløsningsteknikker
```js
function sorter( tall1, tall2, tall3 ) {
}
```
Eksempel 6 i kapittel 8 - Problemløsningsteknikker
```js
function sorter( tall1, tall2, tall3 ) {
    if (tall1 <= tall2 && tall1 <= tall3) {
        // tall1 er først
    } else if (tall2 <= tall3) {
        // tall2 er først
    } else {
        // tall3 er først
    }
}
```
Eksempel 7 i kapittel 8 - Problemløsningsteknikker
```js
function sorter( tall1, tall2, tall3 ) {
    if (tall1 <= tall2 && tall1 <= tall3) {
        if (tall2 <= tall3) {
            // rekkefølgen er tall1, tall2, tall3 
        } else {
            // rekkefølgen er tall1, tall3, tall2
        }
    } else if (tall2 <= tall3) {
        if (tall1 <= tall3) {
            // rekkefølgen er tall2, tall1, tall3
        } else {
            // rekkefølgen er tall2, tall3, tall1
        }
    } else {
        if (tall1 <= tall2) {
            // rekkefølgen er tall3, tall1, tall2
        } else {
            // rekkefølgen er tall3, tall2, tall1
        }
    }
}
```
Eksempel 8 i kapittel 8 - Problemløsningsteknikker
```
> liste = ['Per','Pål', 'Espen']
  (3) ["Per", "Pål", "Espen"]
```
Eksempel 9 i kapittel 8 - Problemløsningsteknikker
```
> liste.splice(1)
  (2) ["Pål", "Espen"]
```
Eksempel 10 i kapittel 8 - Problemløsningsteknikker
```
> liste
  ["Per"]
```
## 9 - Model View Controller
Eksempel 1 i kapittel 9 - Model View Controller
```html
<div id="smiley" onclick="klikk()"></div>
<div id="poeng"></div>
<button onclick="kjøpOppgradering()">Kjøp oppgradering (10 poeng)</button>
```
Eksempel 2 i kapittel 9 - Model View Controller
```html
<style>
    div {
        font-size: 500%;
        user-select: none;
    }
</style>
```
Eksempel 3 i kapittel 9 - Model View Controller
```js
// model
var poeng = 0;
var poengPerKlikk = 1;
var visFørsteSmiley = true;
```
Eksempel 4 i kapittel 9 - Model View Controller
```js
// view
var smileyDiv = document.getElementById('smiley');
var poengDiv = document.getElementById('poeng');

vis();
function vis() {
    smileyDiv.innerHTML = visFørsteSmiley ? '😀' : '😃';
    poengDiv.innerHTML = points;
}
```
Eksempel 5 i kapittel 9 - Model View Controller
```js
function klikk() {
    poeng += poengPerKlikk;
    visFørsteSmiley = !visFørsteSmiley;
    vis();
}

function kjøpOppgradering() {
    if (poeng < 10) return;
    poeng -= 10;
    poengPerKlikk++;
    vis();
}
```
## 10 - Løkker
Eksempel 1 i kapittel 10 - Løkker
```js
if (confirm('Vil du fortsette?')) {
    alert('Hurra!');
}
```
Eksempel 2 i kapittel 10 - Løkker
```js
while (confirm('Vil du fortsette?')) {
    alert('Hurra!');
}
```
Eksempel 3 i kapittel 10 - Løkker
```js
var tall = 1;
while (tall < 10) {
    document.body.innerHTML += tall + ' ';
    tall++;
}
```
Eksempel 4 i kapittel 10 - Løkker
```js
for (var tall = 1; tall < 10; tall++) {
    document.body.innerHTML += tall + ' ';
}
```
Eksempel 5 i kapittel 10 - Løkker
```js
for (;confirm('Vil du fortsette?');) {
    alert('Hurra!');
}
```
Eksempel 6 i kapittel 10 - Løkker
```js
for (var tall = 100; tall < 200; tall += 7) {
    document.body.innerHTML += tall + ' ';
}
```
Eksempel 7 i kapittel 10 - Løkker
```js
function visTall(førsteTall, sisteTall, endring) {
    for (var tall = førsteTall; tall <= sisteTall; tall += endring) {
        document.body.innerHTML += tall + ' ';
    }
}
```
Eksempel 8 i kapittel 10 - Løkker
```js
function visTall(tall, antallTall, endring) {
    while (antallTall > 0) {
        document.body.innerHTML += tall + ' ';
        tall += endring;
        antallTall--;
    }
}
```
Eksempel 9 i kapittel 10 - Løkker
```js
function visTall(tall, antallTall, endring) {
    do {
        document.body.innerHTML += tall + ' ';
        tall += endring;
        antallTall--;
    } while (antallTall > 0);
}
```
## 11 - Lister
Eksempel 1 i kapittel 11 - Lister
```js
let navn = ['Per', 'Pål', 'Espen'];
```
Eksempel 2 i kapittel 11 - Lister
```js
let navn = [];
navn[0] = 'Per';
navn[1] = 'Pål';
navn[2] = 'Espen';
```
Eksempel 3 i kapittel 11 - Lister
```js
var html = '<ul>';
for(let indeks = 0; indeks < navn.length; indeks++) {
    html+= `<li>${navn[indeks]}</li>`;
}
html += '</ul>';
document.getElementById('enId').innerHTML = html;
```
Eksempel 4 i kapittel 11 - Lister
```js
let alleNavn = ['Per', 'Pål', 'Espen'];
var html = '<ul>';
for(let indeks = 0; indeks < alleNavn.length; indeks++) {
    const personNavn = alleNavn[indeks];
    html+= `<li>${personNavn}</li>`;
}
html += '</ul>';
document.getElementById('enId').innerHTML = html;
```
Eksempel 5 i kapittel 11 - Lister
```js
for(let personNavn of alleNavn) {
    html+= `<li>${personNavn}</li>`;
}
```
Eksempel 6 i kapittel 11 - Lister
```js
let obj = { a: 1, b: 2, c: 3 };
for (let felt in obj) {
    let verdi = obj[felt];
    console.log(`${felt}=${verdi}`);
}
```
Eksempel 7 i kapittel 11 - Lister
```js
liste.splice(3, 1);
```
Eksempel 8 i kapittel 11 - Lister
```js
tall.splice(7, 0, 1, 2, 3);
```
Eksempel 9 i kapittel 11 - Lister
```js
var antall = 0;
for(let indeks = 0; indeks < alleTall.length; indeks++){
    const tall = alleTall[indeks];
    if(tall == 7) {
        antall++;
    }
}
let harSju = antall > 0;
```
Eksempel 10 i kapittel 11 - Lister
```js
function harListenVerdien(minListe, søkeVerdi) {
    for(let indeks = 0; indeks < minListe.length; indeks++){
        const verdi = myArray[indeks];
        if(verdi == søkeVerdi) {
            return true;
        }
    }
    return false;
}
```
Eksempel 11 i kapittel 11 - Lister
```js
function filtrerTallOverGrense(minListe, grense) {
    let filtrertListe = [];
    for(let indeks = 0; indeks < minListe.length; indeks++){
        const tall = minListe[index];
        if(tall >= grense) {
            filtrertListe.push(tall);
        }
    }
    return filtrertListe;
}
```
Eksempel 12 i kapittel 11 - Lister
```js
function finnSum(minListe) {
    let sum = 0;
    for(let indeks = 0; indeks < minListe.length; indeks++) {
        const tall = minListe[indeks];
        sum += tall; 
    }
    return sum;
}
```
Eksempel 13 i kapittel 11 - Lister
```js
function getMax(minListe) {
    if(minListe.length == 0) return null;
    let max = minListe[0];
    for(let indeks = 1; indeks < minListe.length; indeks++) {
        const number = minListe[indeks];
        if(number > max) {
            max = number;
        }
    }
    return max;
}
```
Eksempel 14 i kapittel 11 - Lister
```js
function finnGjennomsnitt(minListe) {
    return finnSum(minListe) / minListe.length;
}
```
Eksempel 15 i kapittel 11 - Lister
```js
let liste1 = [1,2,3];
let liste2 = liste1;
liste1[0] = 5;
```
## 12 - Funksjonell programmering
Eksempel 1 i kapittel 12 - Funksjonell programmering
```js
function areal(lengde, bredde) {
    return lengde * bredde;
}
```
Eksempel 2 i kapittel 12 - Funksjonell programmering
```js
function (lengde, bredde) {
    return lengde * bredde;
}
```
Eksempel 3 i kapittel 12 - Funksjonell programmering
```js
let beregnetAreal = function (lengde, bredde) {
                        return lengde * bredde;
                    }(3, 4);
```
Eksempel 4 i kapittel 12 - Funksjonell programmering
```js
const areal = function (lengde, bredde) {
    return lengde * bredde;
}
```
Eksempel 5 i kapittel 12 - Funksjonell programmering
```js
const areal = (lengde, bredde) => lengde * bredde;
```
Eksempel 6 i kapittel 12 - Funksjonell programmering
```js
const kvadrat = side => side * side;
const tilfeldigTerningVerdi = ()) => Math.ceil(Math.random() * 6);
```
Eksempel 7 i kapittel 12 - Funksjonell programmering
```js
const html = (tagNavn, innhold) => `<${tagNavn}>${innhold}</${tagNavn}>`;
```
Eksempel 8 i kapittel 12 - Funksjonell programmering
```js
const html = tagNavn => innhold => `<${tagNavn}>${innhold}</${tagNavn}>`;
```
Eksempel 9 i kapittel 12 - Funksjonell programmering
```js
const h3 = html('h3');
const b = html('b');
```
Eksempel 10 i kapittel 12 - Funksjonell programmering
```js
function filtrerTallOverGrense(minListe, grense) {
    let filtrertListe = [];
    for(let indeks = 0; indeks < minListe.length; indeks++){
        const tall = minListe[index];
        if(tall >= grense) {
            filtrertListe.push(tall);
        }
    }
    return filtrertListe;
}
```
Eksempel 11 i kapittel 12 - Funksjonell programmering
```js
function filtrerTallOverGrense(minListe, grense) {
    return minListe.filter(tall => tall >= grense);
}
```
Eksempel 12 i kapittel 12 - Funksjonell programmering
```js
let alleNavnUpperCase = alleNavn.map(n=>n.toUpperCase());
```
Eksempel 13 i kapittel 12 - Funksjonell programmering
```js
let kurs = 8.57;
let beløpNOK = beløpUSD.map(b => b*kurs);
```
Eksempel 14 i kapittel 12 - Funksjonell programmering
```js
let tall = [3,7];
let sum = tall.reduce((sum, tall)=>tall+sum, 0);
```
Eksempel 15 i kapittel 12 - Funksjonell programmering
```js
let alleNavn = ['Per', 'Pål', 'Espen'];
let html = alleNavn.reduce((htmlListe, navn)=>htmlListe + `<li>${navn}</li>`, '<ul>') + '</ul>';
```
## 13 - Objekter
Eksempel 1 i kapittel 13 - Objekter
```html
<input type="tall" onkeydown="if (event.code === 'Enter') leggTilTall(this);" />
<div id="statistikk"></div>
<script>
    // Model
    var tall = [];

    // Controller
    function leggTilTall(inputTag) {
        tall.push(parseInt(inputTag.value));
        inputTag.value = '';
        vis();
    }

    // View
    var statsDiv = document.getElementById('statistikk');
    function vis() {
        const tallHtml = `<ul>${tall.map(n => `<li>${n}</li>`).join('')}</ul>`;
        var min = tall[0];
        var max = tall[0];
        var sum = 0;
        for (let n of tall) {
            if (n < min) min = n;
            if (n > max) max = n;
            sum += n;
        }
        var gjennomsnitt = sum / numbers.length;
        const statsHtml = 
            `<table>
                <tr><td>Min</td><td>${min}</td></tr>
                <tr><td>Max</td><td>${max}</td></tr>
                <tr><td>Sum</td><td>${sum}</td></tr>
                <tr><td>Snitt</td><td>${avg}</td></tr>
                <tr><td>Antall</td><td>${numbers.length}</td></tr>
            </table>`;
        statsDiv.innerHTML = statsHtml + tallHtml;
    }
</script>    
```
Eksempel 2 i kapittel 13 - Objekter
```js
let person = {};
person.navn = 'Terje';
person.by = 'Stavern';
```
Eksempel 3 i kapittel 13 - Objekter
```js
let person = {
    navn: 'Terje',
    by: 'Stavern',
};
```
Eksempel 4 i kapittel 13 - Objekter
```js
let navn = 'Terje';
let by = 'Stavern';
let person = {navn, by};
```
Eksempel 5 i kapittel 13 - Objekter
```js
function lagStatistikk() {
    var stats = {};
    stats.min = tall[0];
    stats.max = tall[0];
    stats.sum = 0;
    for (let n of tall) {
        if (n < stats.min) stats.min = n;
        if (n > stats.max) stats.max = n;
        stats.sum += n;
    }
    stats.antall = tall.length;
    stats.gjennomsnitt = stats.sum / stats.count;
    return stats;
}
```
Eksempel 6 i kapittel 13 - Objekter
```js
function vis() {
    const tallHtml = `<ul>${tall.map(n => `<li>${n}</li>`).join('')}</ul>`;
    const stats = lagStatistikk();
    const statsHtml = 
        `<table>
            <tr><td>Min</td><td>${stats.min}</td></tr>
            <tr><td>Max</td><td>${stats.max}</td></tr>
            <tr><td>Sum</td><td>${stats.sum}</td></tr>
            <tr><td>Snitt</td><td>${stats.gjennomsnitt}</td></tr>
            <tr><td>Antall</td><td>${stats.antall}</td></tr>
        </table>`;
    statsDiv.innerHTML = statsHtml + tallHtml;
}
```
Eksempel 7 i kapittel 13 - Objekter
```js
// model
var oppgaver = [
    { beskrivelse: 'Handle til middag', erGjort: true },
    { beskrivelse: 'Lage middag', erGjort: false },
    { beskrivelse: 'Spise middag', erGjort: false },
];
```
Eksempel 8 i kapittel 13 - Objekter
```html
<table id="oppgaveTabell"></table>
<p>
    <input id="oppgaveBeskrivelse" type="text"/>
    <button onclick="leggTilOppgave()">Legg til oppgave</button>
</p>
```
Eksempel 9 i kapittel 13 - Objekter
```js
// controller
var beskrivelseInput = document.getElementById('oppgaveBeskrivelse');

function leggTilOppgave() {
    const nyOppgave = {
        beskrivelse: beskrivelseInput.value,
        erGjort: false
    };
    oppgaver.push(nyOppgave);
    beskrivelseInput.value = '';
    vis();
}
```
Eksempel 10 i kapittel 13 - Objekter
```js
function endreErGjort(checkbox, indeks) {
    oppgaver[indeks].erGjort = checkbox.checked;
    vis();
}
```
Eksempel 11 i kapittel 13 - Objekter
```js
function slettOppgave(indeks) {
    oppgaver.splice(indeks, 1);
    vis();
}
```
Eksempel 12 i kapittel 13 - Objekter
```js
function redigerOppgave(indeks) {
    oppgaver[indeks].redigeringsModus = true;
    vis();
}
```
Eksempel 13 i kapittel 13 - Objekter
```js
function lagreOppgave(indeks) {
    const id = `redigerOppgave${indeks}`;
    const inputTag = document.getElementById(id);
    const oppgave = oppgaver[indeks];
    oppgave.beskrivelse = inputTag.value;
    oppgave.redigeringsModus = false;
    vis();
}
```
Eksempel 14 i kapittel 13 - Objekter
```js
// view
var oppgaveTabell = document.getElementById('tasksTable');
vis();

function vis() {
    let html = `<tr>
                    <th>Oppgave</th>
                    <th>Gjort</th>
                    <th></th>
                </tr>`;
    for (let i = 0; i < oppgaver.length; i++) {
        html += lagHtmlRad(i);
    }
    oppgaveTabell.innerHTML = html;
}

function lagHtmlRad(i) {
    const oppgave = oppgaver[i];
    const avkryssetHtml = oppgave.erGjort ? 'checked="checked"' : '';
    const kolonner = oppgave.redigeringsModus
        ? `<td><input id="redigerOppgave${i}" type="text" value="${oppgave.beskrivelse}"/></td>
            <td><input onchange="endreErGjort(this, ${i})" type="checkbox" ${avkryssetHtml} /></td>
            <td>
                <button onclick="lagreOppgave(${i})">Lagre</button>
            </td>`
        : `<td>${oppgave.beskrivelse}</td>
            <td><input onchange="endreErGjort(this, ${i})" type="checkbox" ${avkryssetHtml} /></td>
            <td>
                <button onclick="slettOppgave(${i})">Slett</button>
                <button onclick="redigerOppgave(${i})">Rediger</button>
            </td>`;
    return `<tr>${kolonner}</tr>`;
}
```
Eksempel 15 i kapittel 13 - Objekter
```css
    table, tr, td, th {
        border: 1px solid lightgray;
        border-collapse: collapse;
    }
    td, th {
        padding: 4px;
    }
    th {
        background-color: darkblue;
        border: 1px solid darkblue;
        color: white;
    }
    tr:nth-child(even) {
        background: antiquewhite;
    }
```
Eksempel 16 i kapittel 13 - Objekter
```html
<head>
    <link rel="stylesheet" href="css/vinlotterix.css" />
    <script src="js/model.js"></script>
    <script src="js/common.js"></script>
    <script src="js/personer.js"></script>
    <script src="js/vinnere.js"></script>
</head>
```
Eksempel 17 i kapittel 13 - Objekter
```html
<div class="page" id="page">
    <div class="header" id="header">
        <button class="knapp" onclick="visOgSkjulMeny()">☰</button> Vinlotterix 🍷
    </div>
    <div class="innhold" id="innhold"></div>
    <div class="meny" id="meny">
        <button class="knapp fixed" onclick="visPersoner()">Personer</button><br />
        <button class="knapp fixed" onclick="visTrekninger()">Vinnere</button><br />
    </div>
</div>
```
Eksempel 18 i kapittel 13 - Objekter
```js
visPersoner();

function visOgSkjulMeny() {
    document.getElementById('page').classList.toggle('pageUtenMeny');
}
```
Eksempel 19 i kapittel 13 - Objekter
```js
function visTrekninger() {
  let html = '';
  let cssClass = 'førsteTrekning';
  for (let trekning of model.trekninger) {
    const tid = new Date(trekning.tid);
    const datoTekst = lagDatoTekstForVisning(tid);
    const ukedag = dagsNavn[tid.getDay()];
    const vinnere = trekning.vinnere;
    const deltakere = trekning.deltakere;
    const vinnerOrd = vinnere.length === 1 ? 'Vinneren' : 'Vinnerne';

    html +=
      `<p>
          <small>${ukedag} ${datoTekst}</small><br/>
          <b class="${cssClass}">${vinnerOrd} er ${lagTekstListe(vinnere)}!</b><br/>
          <small>Trukket fra totalt ${deltakere.length} personer: ${lagTekstListe(deltakere)}</small>
      </p>`;
    cssClass = '';
  }
  document.getElementById('innhold').innerHTML = html;
}
```
Eksempel 20 i kapittel 13 - Objekter
```js
liste.splice(3, 1);
```
Eksempel 21 i kapittel 13 - Objekter
```js
tall.splice(7, 0, 
    {fornavn: 'Per', etternavn: 'Olsen'},
    {fornavn: 'Pål', etternavn: 'Nilsen'},
    {fornavn: 'Espen', etternavn: 'Hansen'});
```
Eksempel 22 i kapittel 13 - Objekter
```js
let tall = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
tall.sort()
```
Eksempel 23 i kapittel 13 - Objekter
```js
tall.sort((a, b) => a === b ? 0 : a < b ? -1 : 1);
```
Eksempel 24 i kapittel 13 - Objekter
```js
tall.sort((a, b) => a - b);
```
Eksempel 25 i kapittel 13 - Objekter
```js
tall.sort((a, b) => b - a);
```
Eksempel 26 i kapittel 13 - Objekter
```js
let personer = [    
    {fornavn: 'Per', etternavn: 'Olsen', alder: 19},
    {fornavn: 'Pål', etternavn: 'Nilsen', alder: 18},
    {fornavn: 'Espen', etternavn: 'Hansen', alder: 17}
];
personer.sort((a, b) => a.alder - b.alder);
```
Eksempel 27 i kapittel 13 - Objekter
```js
personer.sort(((a,b) => a.etternavn === b.etternavn ? 0 : 
                        a.etternavn < b.etternavn ? 1 : -1);
```
Eksempel 28 i kapittel 13 - Objekter
```js
personer.sort(((a,b) => a.etternavn.localCompare(b.etternavn));
```
Eksempel 29 i kapittel 13 - Objekter
```js
personer.sort((a, b) => {
  let step1 = a.etternavn.localeCompare(b.etternavn);
  return step1 != 0 ? step1 : a.fornavn.localeCompare(b.fornavn);
});
```
Eksempel 30 i kapittel 13 - Objekter
```js
personer.sort((a, b) => a.etternavn.localeCompare(b.etternavn) 
                     || a.fornavn.localeCompare(b.fornavn));
```
Eksempel 31 i kapittel 13 - Objekter
```js
let personerUnder18 = personer.filter(p => p.alder < 18);
```
Eksempel 32 i kapittel 13 - Objekter
```js
let hansens = personer.filter(p => p.etternavn === 'Hansen');
```
Eksempel 33 i kapittel 13 - Objekter
```js
let person = personer.filter(p => p.id === 1037)[0];
```
Eksempel 34 i kapittel 13 - Objekter
```js
let listeFulleNavn = personer.map(p => p.fornavn + ' ' + p.etternavn);
```
Eksempel 35 i kapittel 13 - Objekter
```js
let listeAldersverdier = personer.map(p => p.alder);
```
Eksempel 36 i kapittel 13 - Objekter
```js
let sumAvAlder = personer.reduce((sum, p) => p.alder + sum, 0);
```
Eksempel 37 i kapittel 13 - Objekter
```js
personer.reduce((max, p) => Math.max(p.alder, max), 0);
```
## 14 - Callbacks, promises og asynkrone kall
Eksempel 1 i kapittel 14 - Callbacks, promises og asynkrone kall
```html
<button onclick="select(this)" disabled="disabled">1</button>
<button onclick="select(this)" disabled="disabled">2</button>
<button onclick="select(this)" disabled="disabled">3</button>

<script>
    enableRandom();
    function select(btn) {
        btn.setAttribute('disabled', 'disabled');
        enableRandom();
    }

    function enableRandom() {
        let btns = document.getElementsByTagName('button');
        let randomIndex = Math.floor(Math.random() * btns.length);
        let btn = btns[randomIndex];
        btn.removeAttribute('disabled');
    }
</script>
```
Eksempel 2 i kapittel 14 - Callbacks, promises og asynkrone kall
```html
<div id="minDiv"></div>
<button onclick="bestillPizza()">Bestill pizza</button>
<script>
    var minDiv = document.getElementById('minDiv');

    function bestillPizza() {
        minDiv.innerHTML = lagPizza();
    }

    function lagPizza() {
        return '<img width="400" src="http://storage.googleapis.com/bro-cdn1/zgrid/themes/10307/images/home/pizza.png"/>';
    }
</script>
``` 
Eksempel 3 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
var minDiv = document.getElementById('minDiv');

function bestillPizza() {
    lagPizza(taImotPizza);
}

function taImotPizza(pizza) {
    minDiv.innerHTML = pizza;
}

function lagPizza(callback) {
    let html = '<img width="400" src="http://storage.googleapis.com/bro-cdn1/zgrid/themes/10307/images/home/pizza.png"/>';
    callback(html);
}
```
Eksempel 4 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
function bestillPizza() {
    lagPizza(pizza => minDiv.innerHTML = pizza);
}

function lagPizza(callback) {
    let html = '<img width="400" src="http://storage.googleapis.com/bro-cdn1/zgrid/themes/10307/images/home/pizza.png"/>';
    callback(html);
}
``` 
Eksempel 5 i kapittel 14 - Callbacks, promises og asynkrone kall
```html
<button id="minKnapp" onclick="gjørNoe()">Trykk på meg!</button>

<script>
    function gjørNoe() {
        // ...
    }
</script>
```
Eksempel 6 i kapittel 14 - Callbacks, promises og asynkrone kall
```html
<button id="minKnapp">Trykk på meg!</button>

<script>
    let minKnapp = document.getElementById('minKnapp');
    minKnapp.onclick = gjørNoe;

    function gjørNoe() {
        // ...
    }
</script>
```
Eksempel 7 i kapittel 14 - Callbacks, promises og asynkrone kall
```html
<button id="minKnapp">Trykk på meg!</button>

<script>
    let minKnapp = document.getElementById('minKnapp');
    minKnapp.addEventListener('click', gjørNoe);

    function gjørNoe() {
        // ...
    }
</script>
```
Eksempel 8 i kapittel 14 - Callbacks, promises og asynkrone kall
```html
<input type="number" id="tall" />
<button onclick="startFaktorisering()">Finn primtallsfaktorene!</button>
<div id="resultat"></div>
<script>
    function startFaktorisering() {
        let tall = parseInt(document.getElementById('tall').value);
        let faktorisert = faktoriser(tall);
        document.getElementById('resultat').innerHTML += faktorisert + '<br/>';
    }

    function faktoriser(tall) {
        let resultat = tall;
        let faktor = 2;
        while (tall > 1) {
            if (tall % faktor == 0) {
                resultat += '⋅' + faktor;
                tall /= faktor;
            } else {
                faktor++;
            }
        }
        return resultat.replace('⋅', '=');
    }
</script>
```
Eksempel 9 i kapittel 14 - Callbacks, promises og asynkrone kall
```html
<input type="number" id="tall" />
<button onclick="startFaktorisering()">Finn primtallsfaktorene!</button>
<div id="resultat"></div>
<script>
    let webworkerCode = `
        function faktoriser(message) {
            let tall = message.data;
            let resultat = '' + tall;
            let faktor = 2;
            while (tall > 1) {
                if (tall % faktor == 0) {
                    resultat += '⋅' + faktor;
                    tall /= faktor;
                } else {
                    faktor++;
                }
            }
            postMessage(resultat.replace('⋅', '='));
        }

        onmessage = faktoriser;`;

    var blob = new Blob([webworkerCode], { type: "application/javascript" });
    var worker = new Worker(URL.createObjectURL(blob));
    worker.onmessage = visResultat;

    function startFaktorisering() {
        let tall = parseInt(document.getElementById('tall').value);
        worker.postMessage(tall);
    }

    function visResultat(message) {
        let resultat = message.data;
        document.getElementById('resultat').innerHTML += resultat + '<br/>';
    }
</script>
```
Eksempel 10 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
posisjon(function (posisjon) {
    sted(posisjon, function(sted){
        værvarsel(sted, function (varselet){
            document.getElementById('varsel').innerHTML = varselet;
        })
    });
});
```
Eksempel 11 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
posisjonPromise()
    .then(posisjon => stedPromise(posisjon))
    .then(sted => værvarselPromise(sted))
    .then(varsel => document.getElementById('varsel').innerHTML = varsel)
    .catch(error => console.error(error));
```
Eksempel 12 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
function stedPromise(posisjon) {
    return new Promise(function (resolve, reject) {
        sted(posisjon, function (sted) {
            resolve(sted);
        });
    });
}
```
Eksempel 13 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
function stedPromise(posisjon) {
    return new Promise(function (resolve, reject) {
        sted(posisjon, function (error, sted) {
            if(error)reject
            resolve(sted);
        });
    });
}
```
Eksempel 14 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
function finnVærvarsel() {
    posisjonPromise()
        .then(posisjon => stedPromise(posisjon))
        .then(sted => værvarselPromise(sted))
        .then(varsel => document.getElementById('varsel').innerHTML = varsel)
}
```
Eksempel 15 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
async function finnVærvarsel() {
    let posisjon = await posisjonPromise();
    let sted = await stedPromise(posisjon);
    let varsel = await værvarselPromise(sted);
    document.getElementById('varsel').innerHTML = varsel;
}
```
Eksempel 16 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
function finnVærvarsel() {
    posisjonPromise()
        .then(posisjon => stedPromise(posisjon))
        .then(sted => værvarselPromise(sted))
        .then(varsel => document.getElementById('varsel').innerHTML = varsel)
        .catch(error => console.error(error));
}
```
Eksempel 17 i kapittel 14 - Callbacks, promises og asynkrone kall
```js
async function finnVærvarsel() {
    try {
        let posisjon = await posisjonPromise();
        let sted = await stedPromise(posisjon);
        let varsel = await værvarselPromise(sted);
        document.getElementById('varsel').innerHTML = varsel;
    } catch (error) {
        console.log(error);
    }
}
```
Eksempel 18 i kapittel 14 - Callbacks, promises og asynkrone kall
```html
<div id="txt"></div>
<script>
    var txtDiv = document.getElementById('txt');
    animate();
    async function animate() {
        try {
            await bokstav('T', 300);
            await bokstav('e', 300);
            await bokstav('?', 300);
            await bokstav('j', 300);
            await bokstav('e', 300);
        } catch{
            txt.innerHTML = "Error!!!";
        }
    }
    function bokstav(txt, millis) {
        return new Promise(function (resolve, reject) {
            setTimeout(function () {
                if (txt == '?') reject();
                txtDiv.innerHTML += txt;
                resolve();
            }, millis);
        });
    }
</script>
```
## 15 - Backend med Google Firebase
Eksempel 1 i kapittel 15 - Backend med Google Firebase
```html
<script src="https://www.gstatic.com/firebasejs/6.3.1/firebase-app.js"></script>
<script>
  var firebaseConfig = {
    apiKey: "AbCdEfGhIjKlMpWhV7Tj-NrxWUQ1S-EsUicEE23",
    authDomain: "kodingforalle.firebaseapp.com",
    databaseURL: "https://kodingforalle.firebaseio.com",
    projectId: "kodingforalle",
    storageBucket: "kodingforalle.appspot.com",
    messagingSenderId: "123456789012",
    appId: "1:123456543212:web:084e23f1e2295463"
  };
  firebase.initializeApp(firebaseConfig);
</script>
```
Eksempel 2 i kapittel 15 - Backend med Google Firebase
```html
<html>
<head>
    <script src="https://www.gstatic.com/firebasejs/6.3.1/firebase-app.js"></script>
    <script src="https://www.gstatic.com/firebasejs/6.3.1/firebase-firestore.js"></script>
</head>
<body>
    <script>
        var firebaseConfig = { /* behold ditt eget oppsett her */};

        firebase.initializeApp(firebaseConfig);
        let db = firebase.firestore();
        lesDokument('xwBymPkcAqCLlEkwJjD2' /* bytt ut med din egen id her */ );

        async function lesDokument(id) {
            try {
                let kommentarCollection = db.collection('kommentarer');
                let dokumentReferanse = kommentarCollection.doc(id);
                let dokumentSnapshot = await dokumentReferanse.get();
                let dokument = dokumentSnapshot.data();
                console.log(dokument);
            } catch (error) {
                console.error(error);
            }
        }
    </script>
</body>
</html>
```
Eksempel 3 i kapittel 15 - Backend med Google Firebase
```js
{
    forfatter: "Terje",
    tekst: "Testkommentar",
    tid: {
        seconds: 1563953400,
        nanoseconds: 0
    }
}
```
Eksempel 4 i kapittel 15 - Backend med Google Firebase
```js
let kommentarCollection = db.collection('kommentarer');
let dokumentReferanse = kommentarCollection.doc(id);
unsubscribe = await dokumentReferanse.onSnapshot(
    function (dokumentSnapshot) {
        let dokument = dokumentSnapshot.data();
        console.log(dokument);
    });
```
Eksempel 5 i kapittel 15 - Backend med Google Firebase
```js
async function testAvAdd() {
    try {
        let dokument = { tekst: 'add', forfatter: 'Per', tid: new Date() };
        let dokumentSnapshot = await db.collection('kommentarer').add(dokument);
        let id = dokumentSnapshot.id;
    } catch (error) {
        console.error(error);
    }
}
```
Eksempel 6 i kapittel 15 - Backend med Google Firebase
```js
async function testAvSet() {
    try {
        let dokument = { tekst: 'test av set' };
        let dokumentSnapshot = await db.collection('kommentarer').doc('xwBymPkcAqCLlEkwJjD2');
        await dokumentSnapshot.set(dokument);
    } catch (error) {
        console.error(error);
    }
}
```
Eksempel 7 i kapittel 15 - Backend med Google Firebase
```js
async function lesAlleDokumentene() {
    let kommentarCollection = db.collection('kommentarer');
    let collectionSnapshot = await kommentarCollection.get();
    let collection = collectionSnapshot.docs.map(dokumentSnapshot => dokumentSnapshot.data());
}
```
Eksempel 8 i kapittel 15 - Backend med Google Firebase
```js
async function lesAlleDokumentene() {
    let kommentarCollection = db.collection('kommentarer');
    let collectionSnapshot = await kommentarCollection.get();
    for (let dokumentSnapshot of collectionSnapshot.docs) {
        let dokument = dokumentSnapshot.data();
        /* ... gjøre noe med hvert dokument */
    }
}
```
Eksempel 9 i kapittel 15 - Backend med Google Firebase
```js
let kommentarCollection = db.collection('kommentarer');
let query = kommentarCollection.where('forfatter', '==', 'Terje')
let collectionSnapshot = await query.get();
```
Eksempel 10 i kapittel 15 - Backend med Google Firebase
```js
async function hentDataFraFirestore() {
  try {
    let personerDoc = await db.collection('personer').orderBy('navn').get();
    model.personer.liste = personerDoc.docs.map(mapPerson);
    let trekningerDoc = await db.collection('trekninger').orderBy('tid', 'desc').get();
    model.trekninger = trekningerDoc.docs.map(mapTrekning);
    visPersoner();
  } catch (error) {
    console.error(error);
  }
}
```
Eksempel 11 i kapittel 15 - Backend med Google Firebase
```js
function mapPerson(personDoc) {
  let personObj = personDoc.data();
  personObj.id = personDoc.id;
  personObj.erValgt = true;
  return personObj;
}

function mapTrekning(trekningDoc) {
  let trekningObj = trekningDoc.data();
  trekningObj.tid = trekningObj.tid.toDate().toISOString().substr(0,16);
  return trekningObj;
}
```
Eksempel 12 i kapittel 15 - Backend med Google Firebase
```js
async function leggTilPerson() {
  const navn = document.getElementById('nyPerson').value;
  try {
    let personObj = await db.collection('personer').add({ navn });
    model.personer.liste.push(
      { id: personObj.id, navn: navn, erValgt: true });
    visPersoner();
  } catch (error) {
    console.error(error);
  }
}
```
Eksempel 13 i kapittel 15 - Backend med Google Firebase
```js
try {
    let trekningKopi = JSON.parse(JSON.stringify(nyTrekning));
    trekningKopi.tid = new Date(trekningKopi.tid);
    await db.collection('trekninger').add(trekningKopi);
    model.trekninger.unshift(nyTrekning);
    visTrekninger();
} catch (error) {
    console.error(error);
}  
```
## 16 - Mer objektorientert Javascript med klasser
Eksempel 1 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
motor.start();
```
Eksempel 2 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
let ruteH3 = {
    kolonne: 'H',
    rad: 3
};
```
Eksempel 3 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
function kode(rute) {
    return rute.kolonne + rute.rad;
}
```
Eksempel 4 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Rute {
    kode() {
        return this.kolonne + this.rad;
    }
}
```
Eksempel 5 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
let ruteH3 = new Rute();
ruteH3.rad = 3;
ruteH3.kolonne = 'H';
console.log(ruteH3.kode());
```
Eksempel 6 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
let ruteH3 = {};
ruteH3.rad = 3;
ruteH3.kolonne = 'H';
console.log(kode(ruteH3));
```
Eksempel 7 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Rute {
    constructor() {
        console.log('lager nytt objekt av klassen Rute!')
    }

    kode() {
        return this.kolonne + this.rad;
    }
}
```
Eksempel 8 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Rute {
    constructor(kolonne, rad) {
        this.kolonne = kolonne;
        this.rad = rad;
    }

    kode() {
        return this.kolonne + this.rad;
    }
}
```
Eksempel 9 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
let ruteH3 = new Rute('H', 3);
```
Eksempel 10 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Brikke {
    constructor(kolonne, rad) {
        this.kolonne = kolonne;
        this.rad = rad;
    }

    posisjon() {
        return this.kolonne + this.rad;
    }
}
```
Eksempel 11 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Brikke {
    constructor(kolonne, rad) {
        this.flyttTilKolonneOgRad(kolonne, rad);
    }

    posisjon() {
        return this.kolonne + this.rad;
    }

    flyttTilPosisjon(posisjon) {
        this.flyttTilKolonneOgRad(posisjon[0], posisjon[1]);
    }

    flyttTilKolonneOgRad(kolonne, rad) {
        this.kolonne = kolonne;
        this.rad = rad;
    }

    flytt(kolonnerTilHøyre, raderOppover) {
        let tallKodeForKolonne = this.kolonne.charCodeAt(0);
        tallKodeForKolonne += kolonnerTilHøyre;
        this.kolonne = String.fromCharCode(tallKodeForKolonne);
        this.rad += raderOppover;
    }
}
```
Eksempel 12 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Brikke {
    constructor(kolonne, rad) {
        this.flyttTilKolonneOgRad(kolonne, rad);
    }

    flyttTilPosisjon(posisjon) {
        this.posisjon = posisjon;
    }

    flyttTilKolonneOgRad(kolonne, rad) {
        this.posisjon = kolonne + rad;
    }

    flytt(kolonnerTilHøyre, raderOppover) {
        let kolonne = this.posisjon[0];
        let rad = parseInt(this.posisjon[1]);
        let tallKodeForKolonne = kolonne.charCodeAt(0);
        tallKodeForKolonne += kolonnerTilHøyre;
        kolonne = String.fromCharCode(tallKodeForKolonne);
        rad += raderOppover;
        this.flyttTilKolonneOgRad(kolonne, rad);
    }
}
```
Eksempel 13 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Brikke {
    constructor(kolonneBokstav, rad) {
        this.flyttTilKolonneOgRad(kolonneBokstav, rad);
    }

    posisjon() {
        let tallKodeForKolonneA = 'A'.charCodeAt(0);
        let kolonneBokstav = String.fromCharCode(tallKodeForKolonneA + this.kolonne);
        return kolonneBokstav + this.rad;
    }

    flyttTilPosisjon(posisjon) {
        this.flyttTilKolonneOgRad(posisjon[0], posisjon[1]);
    }

    flyttTilKolonneOgRad(kolonneBokstav, rad) {
        this.kolonne = kolonneBokstav.charCodeAt(0) - 'A'.charCodeAt(0);
        this.rad = parseInt(rad);
    }

    flytt(kolonnerTilHøyre, raderOppover) {
        this.kolonne += kolonnerTilHøyre;
        this.rad += raderOppover;
    }
}
```
Eksempel 14 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Brikke {
    constructor(kolonneBokstav, rad, type) {
        this.flyttTilKolonneOgRad(kolonneBokstav, rad);
        this.type = type;
    }

    posisjon() {
        return Brikke.bokstavFraKolonne(this.kolonne) + this.rad;
    }

    flyttTilPosisjon(posisjon) {
        return this.flyttTilKolonneOgRad(posisjon[0], posisjon[1]);
    }

    flyttTilKolonneOgRad(kolonneBokstav, rad) {
        return this.flyttTil(Brikke.kolonneFraBokstav(kolonneBokstav), parseInt(rad));
    }

    flytt(kolonnerTilHøyre, raderOppover) {
        return this.flyttTil(this.kolonne + kolonnerTilHøyre, this.rad + raderOppover);
    }

    flyttTil(kolonne, rad) {
        if (this.type == 'Tårn' && this.kolonne != kolonne && this.rad != rad) return false;
        if (this.type == 'Løper') {
            var diffKolonne = this.kolonne - kolonne;
            var diffRad = this.rad - rad;
            if (Math.Abs(diffRad) != Math.Abs(diffKolonne)) return false;
        }
        this.kolonne = kolonne;
        this.rad = rad;
        return true;
    }

    static kolonneFraBokstav(bokstav) {
        return bokstav.charCodeAt(0) - 'A'.charCodeAt(0);
    }

    static bokstavFraKolonne(kolonne) {
        let tallKodeForKolonneA = 'A'.charCodeAt(0);
        return String.fromCharCode(tallKodeForKolonneA + kolonne);
    }
}
```
Eksempel 15 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Brett {
    constructor() {
        this.brikker = {
            a1: new Brikke('a', 1, 'Tårn'),
            a3: new Brikke('a', 3, 'Løper')
        }
    }

    flytt(fraPosisjon, tilPosisjon) {
        let fraBrikke = this.brikker[fraPosisjon];
        if (!fraBrikke) return false;
        let tilBrikke = this.brikker[tilPosisjon];
        if (tilBrikke) return false;
        let suksess = fraBrikke.flyttTilPosisjon(tilPosisjon);
        if (!suksess) return false;
        delete this.brikker[fraPosisjon];
        this.brikker[tilPosisjon] = fraBrikke;
    }
}
```
Eksempel 16 i kapittel 16 - Mer objektorientert Javascript med klasser
```
Program->Brett: flytt('a1', 'a4')
Brett->Brett: finnBrikke('a1')
Brett->Brikke: flyttTilPosisjon('a4')
```
Eksempel 17 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
flyttTil(kolonne, rad) {
    this.kolonne = kolonne;
    this.rad = rad;
    return true;
}
```
Eksempel 18 i kapittel 16 - Mer objektorientert Javascript med klasser
```js
class Tårn extends Brikke {
    constructor(kolonneBokstav, rad) {
        super(kolonneBokstav, rad, 'Tårn');
    }

    flyttTil(kolonne, rad) {
        if (this.kolonne != kolonne && this.rad != rad) return false;
        return super.flyttTil(kolonne, rad);
    }
}

class Løper extends Brikke {
    constructor(kolonneBokstav, rad) {
        super(kolonneBokstav, rad, 'Løper');
    }

    flyttTil(kolonne, rad) {
        var diffKolonne = this.kolonne - kolonne;
        var diffRad = this.rad - rad;
        if (Math.Abs(diffRad) != Math.Abs(diffKolonne)) return false;
        return super.flyttTil(kolonne, rad);
    }
}
```
## 17 - SPA-rammeverket Vue.js
Eksempel 1 i kapittel 17 - SPA-rammeverket Vue.js
```html
<div id="teller"></div>
<button onclick="leggTil(1)">+</button>
<button onclick="leggTil(-1)">-</button>
<input type="number" id="nyttTall" />
<button onclick="endre()">Endre</button>
<script>
    // View
    let tellerDiv = document.getElementById('teller');
    function visTeller() {
        tellerDiv.innerHTML = teller;
    }

    // Model
    let teller = 0;

    // Controller
    let nyttTallDiv = document.getElementById('nyttTall');
    visTeller();

    function endre() {
        teller = parseInt(nyttTallDiv.value);
        visTeller();
    }

    function leggTil(tall) {
        teller += tall;
        visTeller();
    }
</script>
```
Eksempel 2 i kapittel 17 - SPA-rammeverket Vue.js
```html
<html>
<head>
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
</head>
<body>
    <!-- View -->
    <div id="app">
        <div id="teller">{{ teller }}</div>
        <button @click="teller++">+</button>
        <button @click="teller--">-</button>
        <input v-model="nyttTall" />
        <button @click="teller=parseInt(nyttTall)">Endre</button>
    </div>
    <script>
        var app = new Vue({
            el: '#app',
            data: { // Model
                teller: 0,
                nyttTall: 0
            }
        })
    </script>
</body>
</html>
```
Eksempel 3 i kapittel 17 - SPA-rammeverket Vue.js
```html
<!-- View -->
<div id="app">
    <div id="teller">{{ teller }}</div>
    <button @click="endre(1)">+</button>
    <button @click="endre(-1)">-</button>
    <input v-model="nyttTall" />
    <button @click="kopierNyttTall()">Endre</button>
</div>
<script>
    var app = new Vue({
        el: '#app',
        // Model
        data: {
            teller: 0,
            nyttTall: 0
        },
        methods: {
            endre(endring) {
                this.teller += parseInt(endring);
            },
            kopierNyttTall() {
                this.teller = parseInt(this.nyttTall);
            }
        }
    })
</script>
```
Eksempel 4 i kapittel 17 - SPA-rammeverket Vue.js
```js
methods: {
    endre: function(endring) {
        this.teller += parseInt(endring);
    },
    kopierNyttTall: function() {
        this.teller = parseInt(this.nyttTall);
    }
}
```
Eksempel 5 i kapittel 17 - SPA-rammeverket Vue.js
```html
<!DOCTYPE html>

<html lang="en" xmlns="http://www.w3.org/1999/xhtml">
<head>
    <link rel="stylesheet" href="css/vinlotterix.css" />
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
</head>
<body>
    <div class="page" :class="showMenu ? '' : 'pageUtenMeny'" id="page">
        <div class="header" id="header">
            <button @click="visOgSkjulMeny" class="knapp">☰</button> Vinlotterix 🍷
        </div>
        <div v-if="currentPage == 'personer'" class="innhold" id="innhold">
            <table>
                <tr>
                    <td>
                        <input type="checkbox" v-model="personer.velgAlle"
                               @click="velgAlleEllerIngen" />
                    </td>
                    <td><b>Personer</b></td>
                    <td></td>
                </tr>
                <tr v-for="person in personer.liste">
                    <td>
                        <input type="checkbox" v-model="person.erValgt" />
                    </td>
                    <td>{{person.navn}}</td>
                    <td><button class="litenKnapp" @click="slettPerson(person.id)">x</button></td>
                </tr>
                <tr>
                    <td></td>
                    <td colspan="3">
                        <input size="6" type="text" v-model="personer.nyPerson" />
                        <button class="litenKnapp" @click="leggTilPerson">legg til person</button>
                    </td>
                </tr>
                <tr><td>&nbsp;</td></tr>
                <tr>
                    <td colspan="3">
                        <button class="knapp" @click="trekk">Trekk!</button>
                        <input type="number" size="1" v-model="personer.trekkAntall" />
                        <button class="" @click="personer.trekkAntall++">▲</button>
                        <button class="" @click="personer.trekkAntall = Math.max(1,personer.trekkAntall -1)">▼</button>
                    </td>
                </tr>
            </table>
        </div>
        <div v-else-if="currentPage == 'trekninger'" class="innhold" id="innhold">
            <p v-for="(trekning, i) in trekninger">
                <small>
                    {{dagsNavn[new Date(trekning.tid).getDay()]}}
                    {{lagDatoTekstForVisning(new Date(trekning.tid))}}
                </small><br />
                <b  :class="'førsteTrekning' + i ">
                    {{trekning.vinnere.length === 1 ? 'Vinneren' : 'Vinnerne'}}
                    er {{lagTekstListe(trekning.vinnere)}}!
                </b><br />
                <small>
                    Trukket fra totalt {{trekning.deltakere.length}} personer:
                    {{lagTekstListe(trekning.deltakere)}}
                </small>
            </p>
        </div>
        <div v-if="showMenu" class="meny" id="meny">
            <button class="knapp fixed" @click="currentPage = 'personer'">Personer</button><br />
            <button class="knapp fixed" @click="currentPage = 'trekninger'">Trekninger</button><br />
        </div>
    </div>
    <script>
        var app = new Vue({
            el: '#page',
            data: {
                showMenu: true,
                currentPage: 'personer',
                personer: {
                    nyPerson: '',
                    velgAlle: false,
                    trekkAntall: 1,
                    liste: [
                        { id: 100, navn: 'Per', erValgt: true },
                        { id: 101, navn: 'Pål', erValgt: true },
                        { id: 102, navn: 'Espen', erValgt: false },
                        { id: 103, navn: 'Ole', erValgt: true },
                    ]
                },
                trekninger: [
                    {
                        vinnere: ['Ole'],
                        tid: '2018-10-17 17:10',
                        deltakere: ['Per', 'Pål', 'Ole']
                    }
                    , {
                        vinnere: ['Per', 'Pål', 'Knut'],
                        tid: '2018-10-11 17:10',
                        deltakere: ['Per', 'Pål', 'Ole', 'Knut', 'Gunnar']
                    }
                ],
                dagsNavn: ['søndag', 'mandag', 'tirsdag', 'onsdag', 'torsdag', 'fredag', 'lørdag']
            },
            methods: {
                visOgSkjulMeny() {
                    this.showMenu = !this.showMenu;
                },
                lagTekstListe(liste) {
                    if (liste.length === 0) return '';
                    if (liste.length === 1) return liste[0];
                    const tekstListe = liste.join(', ');
                    const indexSisteKomma = tekstListe.lastIndexOf(',');
                    return tekstListe.substr(0, indexSisteKomma)
                        + ' og ' + tekstListe.substr(indexSisteKomma + 1);
                },
                lagDatoTekstForVisning(dato) {
                    return dato.toLocaleString().replace(',', '').substr(0, 15);
                },
                lagDatoTekstForLagring(dato) {
                    return dato.toISOString().substr(0, 16).replace('T', ' ');
                },
                lagDatoTekstNåForLagring() {
                    return this.lagDatoTekstForLagring(new Date());
                },
                velgAlleEllerIngen() {
                    let verdi = !this.personer.velgAlle;
                    for (let person of this.personer.liste) {
                        person.erValgt = verdi;
                    }
                },
                slettPerson(id) {
                    let index = this.personer.liste.findIndex((p => p.id === id));
                    if (index == -1) return;
                    this.personer.liste.splice(index, 1);
                },
                leggTilPerson() {
                    const id = 1 + this.personer.liste
                        .map(p => p.id).reduce((max, value) => Math.max(max, value), -1);
                    this.personer.liste
                        .push({ id: id, navn: this.personer.nyPerson, erValgt: true });
                },
                trekk() {
                    let antall = this.personer.trekkAntall;
                    const personerListe = this.personer.liste.filter(p => p.erValgt);
                    const indekser = Array.from(personerListe.keys());
                    const vinnere = [];
                    while (antall-- > 0 && indekser.length > 0) {
                        const tilfeldigIndeks = Math.floor(Math.random() * indekser.length);
                        const indeks = indekser.splice(tilfeldigIndeks, 1);
                        vinnere.push(personerListe[indeks].navn);
                    }
                    this.trekninger.unshift({
                        vinnere: vinnere,
                        tid: this.lagDatoTekstNåForLagring(),
                        deltakere: personerListe.map(p => p.navn)
                    });
                    this.currentPage = 'trekninger';
                }
            }
        })
    </script>
</body>
</html>
```
Eksempel 6 i kapittel 17 - SPA-rammeverket Vue.js
```html
<div id="app">
    <div id="teller">{{ teller }}</div>
    <button @click="teller++">+</button>
</div>
<script>
    var app = new Vue({
        el: '#app',
        data: {
            teller: 0
        }
    })
</script>
```
Eksempel 7 i kapittel 17 - SPA-rammeverket Vue.js
```html
<div id="app">
    <super-teller></super-teller>
    <super-teller></super-teller>
</div>
<script>
    Vue.component('super-teller', {
        data() {
            return {
                teller: 0
            };
        },
        template: 
            `<div>
                <div id="teller">{{ teller }}</div>
                <button @click="teller++">+</button>
            </div>`
    });
    var app = new Vue({
        el: '#app'
    })
```
Eksempel 8 i kapittel 17 - SPA-rammeverket Vue.js
```js
Vue.component('super-teller', {
    data() {
        return {
            teller: 0
        };
    },
    methods: {
        tell() {
            this.teller++;
        }
    },
    template:
        `<div>
        <div id="teller">{{ teller }}</div>
        <button @click="tell">+</button>
    </div>`
});
```
Eksempel 9 i kapittel 17 - SPA-rammeverket Vue.js
```html
<super-teller start="1000"></super-teller>
<super-teller start="0"></super-teller>
```
Eksempel 10 i kapittel 17 - SPA-rammeverket Vue.js
```js
Vue.component('super-teller', {
    data() {
        return {
            teller: 0
        };
    },
    props: ['start'],
    methods: {
        tell() {
            this.teller++;
        }
    },
    created() {
        this.teller = this.start;
    },
    template:
        `<div>
            <div id="teller">{{ teller }}</div>
            <button @click="tell">+</button>
         </div>`
});
```
Eksempel 11 i kapittel 17 - SPA-rammeverket Vue.js
```js
Vue.component('person-liste', {
    props: ['personerProp'],
    data() {
        return {
            nyPerson: '',
            velgAlle: false,
            trekkAntall: 1,
            liste: []
        };
    },
    created() {
        this.liste.push(...this.personerProp);
    },
    methods: {
        velgAlleEllerIngen() {
            let verdi = !this.velgAlle;
            for (let person of this.liste) {
                person.erValgt = verdi;
            }
        },
        slettPerson(id) {
            let index = this.liste.findIndex((p => p.id === id));
            if (index == -1) return;
            this.liste.splice(index, 1);
            this.$emit('oppdatert-personliste', this.liste);
        },
        leggTilPerson() {
            const id = this.liste
                .map(p => p.id).reduce((max, value) => Math.max(max, value), -1) + 1;
            this.liste
                .push({ id: id, navn: this.nyPerson, erValgt: true });
            this.nyPerson = '';
            this.$emit('oppdatert-personliste', this.liste);
        },
        trekk() {
            this.$emit('trekk', this.trekkAntall);
        }
    },
    template: `<div class="innhold" id="innhold">
            <table>
                <tr>
                    <td>
                        <input type="checkbox" v-model="velgAlle"
                               @click="velgAlleEllerIngen" />
                    </td>
                    <td><b>Personer</b></td>
                    <td></td>
                </tr>
                <tr v-for="person in liste">
                    <td>
                        <input type="checkbox" v-model="person.erValgt" />
                    </td>
                    <td>{{person.navn}}</td>
                    <td><button class="litenKnapp" @click="slettPerson(person.id)">x</button></td>
                </tr>
                <tr>
                    <td></td>
                    <td colspan="3">
                        <input size="6" type="text" v-model="nyPerson" />
                        <button class="litenKnapp" @click="leggTilPerson">legg til person</button>
                    </td>
                </tr>
                <tr><td>&nbsp;</td></tr>
                <tr>
                    <td colspan="3">
                        <button class="knapp" @click="trekk">Trekk!</button>
                        <input type="number" size="1" v-model="trekkAntall" />
                        <button class="" @click="trekkAntall++">▲</button>
                        <button class="" @click="trekkAntall = Math.max(1,personer.trekkAntall -1)">▼</button>
                    </td>
                </tr>
            </table>
        </div>`
});
```
Eksempel 12 i kapittel 17 - SPA-rammeverket Vue.js
```js
Vue.component('trekning-liste', {
    props: ['trekningerProp'],
    data() {
        return {
            trekninger: [],
            dagsNavn: ['søndag', 'mandag', 'tirsdag', 'onsdag', 'torsdag', 'fredag', 'lørdag']
        }
    },
    created() {
        this.trekninger.push(...this.trekningerProp);
    },
    methods: {
        lagDatoTekstForVisning(dato) {
            return dato.toLocaleString().replace(',', '').substr(0, 15);
        },
        lagTekstListe(liste) {
            if (liste.length === 0) return '';
            if (liste.length === 1) return liste[0];

            const tekstListe = liste.join(', ');
            const indexSisteKomma = tekstListe.lastIndexOf(',');
            return tekstListe.substr(0, indexSisteKomma)
                + ' og ' + tekstListe.substr(indexSisteKomma + 1);
        }
    },
    template: `<div class="innhold" id="innhold">
            <p v-for="(trekning, i) in trekninger">
                <small>
                    {{dagsNavn[new Date(trekning.tid).getDay()]}}
                    {{lagDatoTekstForVisning(new Date(trekning.tid))}}
                </small><br />
                <b :class="'førsteTrekning' + i ">
                    {{trekning.vinnere.length === 1 ? 'Vinneren' : 'Vinnerne'}}
                    er {{lagTekstListe(trekning.vinnere)}}!
                </b><br />
                <small>
                    Trukket fra totalt {{trekning.deltakere.length}} personer:
                    {{lagTekstListe(trekning.deltakere)}}
                </small>
            </p>
        </div>`
});
```
Eksempel 13 i kapittel 17 - SPA-rammeverket Vue.js
```html
<!DOCTYPE html>

<html lang="en" xmlns="http://www.w3.org/1999/xhtml">
<head>
    <link rel="stylesheet" href="css/vinlotterix.css" />
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    <script src="js/person-liste.js"></script>
    <script src="js/trekning-liste.js"></script>
</head>
<body>
    <div class="page" :class="showMenu ? '' : 'pageUtenMeny'" id="page">
        <div class="header" id="header">
            <button @click="visOgSkjulMeny" class="knapp">☰</button> Vinlotterix 🍷
        </div>
        <person-liste v-if="currentPage == 'personer'" 
                      :personer-prop="personer"
                      @trekk="trekk"
                      @oppdatert-personliste="oppdaterPersoner"
                      ></person-liste>
        <trekning-liste v-else-if="currentPage == 'trekninger'" 
                          :trekninger-prop="trekninger"></trekning-liste>

        <div v-if="showMenu" class="meny" id="meny">
            <button class="knapp fixed" @click="currentPage = 'personer'">Personer</button><br />
            <button class="knapp fixed" @click="currentPage = 'trekninger'">Trekninger</button><br />
        </div>
    </div>
    <script>
        var app = new Vue({
            el: '#page',
            data: {
                showMenu: true,
                currentPage: 'personer',
                personer: [
                    { id: 100, navn: 'Per', erValgt: true },
                    { id: 101, navn: 'Pål', erValgt: true },
                    { id: 102, navn: 'Espen', erValgt: false },
                    { id: 103, navn: 'Ole', erValgt: true },
                ],
                trekninger: [
                    {
                        vinnere: ['Ole'],
                        tid: '2018-10-17 17:10',
                        deltakere: ['Per', 'Pål', 'Ole']
                    },
                    {
                        vinnere: ['Per', 'Pål', 'Knut'],
                        tid: '2018-10-11 17:10',
                        deltakere: ['Per', 'Pål', 'Ole', 'Knut', 'Gunnar']
                    }
                ]
            },
            methods: {
                visOgSkjulMeny() {
                    this.showMenu = !this.showMenu;
                },
                lagDatoTekstForLagring(dato) {
                    return dato.toISOString().substr(0, 16).replace('T', ' ');
                },
                lagDatoTekstNåForLagring() {
                    return this.lagDatoTekstForLagring(new Date());
                },
                trekk(antall) {
                    const personerListe = this.personer.filter(p => p.erValgt);
                    const indekser = Array.from(personerListe.keys());
                    const vinnere = [];
                    while (antall-- > 0 && indekser.length > 0) {
                        const tilfeldigIndeks = Math.floor(Math.random() * indekser.length);
                        const indeks = indekser.splice(tilfeldigIndeks, 1);
                        vinnere.push(personerListe[indeks].navn);
                    }
                    this.trekninger.unshift({
                        vinnere: vinnere,
                        tid: this.lagDatoTekstNåForLagring(),
                        deltakere: personerListe.map(p => p.navn)
                    });
                    this.currentPage = 'trekninger';
                },
                oppdaterPersoner(personer) {
                    this.personer.length = 0;
                    this.personer.push(...personer);
                }
            }
        });
    </script>
</body>
</html>
```
Eksempel 14 i kapittel 17 - SPA-rammeverket Vue.js
```js
tell() {
    this.teller++;
    if(this.teller == this.slutt){
        this.$emit('fullført', this.teller);
    }
}
```
Eksempel 15 i kapittel 17 - SPA-rammeverket Vue.js
```html
<div id="app">
    <super-teller @fullført="visEvent" start="0" slutt="4"></super-teller>
    <super-teller @fullført="visEvent" start="0" slutt="5"></super-teller>
</div>
<script>
    Vue.component('super-teller', {
        data() {
            return {
                teller: 0
            };
        },
        props: ['start', 'slutt'],
        methods: {
            tell() {
                this.teller++;
                if (this.teller == this.slutt) {
                    this.$emit('fullført', this.teller);
                }
            }
        },
        created() {
            this.teller = this.start;
        },
        template:
            `<div>
        <div id="teller">{{ teller }}</div>
        <button @click="tell">+</button>
        </div>`
    });
    var app = new Vue({
        el: '#app',
        methods: {
            visEvent(event) {
                console.log('Mottatt fullført: ', event);
            }
        }
    })
</script>
```
Eksempel 16 i kapittel 17 - SPA-rammeverket Vue.js
```
npm install -g @vue/cli
npm install -g @vue/cli-init
```
Eksempel 17 i kapittel 17 - SPA-rammeverket Vue.js
```
vue init webpack vuetest
```
Eksempel 18 i kapittel 17 - SPA-rammeverket Vue.js
```
? Project name vuetest
? Project description A Vue.js project
? Author Terje Kolderup 
? Vue build standalone
? Install vue-router? Yes
? Use ESLint to lint your code? No
? Set up unit tests No
? Setup e2e tests with Nightwatch? No
? Should we run `npm install` for you after the project has been created? (recommended) npm
```
Eksempel 19 i kapittel 17 - SPA-rammeverket Vue.js
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <title>vuetest</title>
  </head>
  <body>
    <div id="app"></div>
    <!-- built files will be auto injected -->
  </body>
</html>
```
Eksempel 20 i kapittel 17 - SPA-rammeverket Vue.js
```html
<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>


<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
```
Eksempel 21 i kapittel 17 - SPA-rammeverket Vue.js
```js
import Vue from 'vue'
import Router from 'vue-router'
import HelloWorld from '@/components/HelloWorld'

Vue.use(Router)

export default new Router({
  routes: [
    {
      path: '/',
      name: 'HelloWorld',
      component: HelloWorld
    }
  ]
})
```
Eksempel 22 i kapittel 17 - SPA-rammeverket Vue.js
```
Hash: dcf1dbd4ce58da2f3196
Version: webpack 3.12.0
Time: 6990ms
                                                  Asset       Size  Chunks             Chunk Names
               static/js/vendor.bc0463846e4fa806a1be.js     121 kB       0  [emitted]  vendor
                  static/js/app.b22ce679862c47a75225.js    11.6 kB       1  [emitted]  app
             static/js/manifest.2ae2e69a05c33dfc65f8.js  857 bytes       2  [emitted]  manifest
    static/css/app.30790115300ab27614ce176899523b62.css  432 bytes       1  [emitted]  app
static/css/app.30790115300ab27614ce176899523b62.css.map  797 bytes          [emitted]
           static/js/vendor.bc0463846e4fa806a1be.js.map     608 kB       0  [emitted]  vendor
              static/js/app.b22ce679862c47a75225.js.map    22.2 kB       1  [emitted]  app
         static/js/manifest.2ae2e69a05c33dfc65f8.js.map    4.97 kB       2  [emitted]  manifest
                                             index.html  509 bytes          [emitted]

  Build complete.

  Tip: built files are meant to be served over an HTTP server.
  Opening index.html over file:// won't work.
```
Eksempel 23 i kapittel 17 - SPA-rammeverket Vue.js
```
DONE  Compiled successfully in 3323ms                             14:55:17
 I  Your application is running here: http://localhost:8080
```
Eksempel 24 i kapittel 17 - SPA-rammeverket Vue.js
```html
<a name="seksjon1"/><p><h1>Seksjon 1</h1>Bla bla bla.<hr style="height: 500px" /></p>
<a name="seksjon2"/><p><h1>Seksjon 2</h1>Bla bla bla.<hr style="height: 500px" /></p>
<a name="seksjon3"/><p><h1>Seksjon 3</h1>Bla bla bla.<hr style="height: 500px" /></p>
```
Eksempel 25 i kapittel 17 - SPA-rammeverket Vue.js
```html
<template>
  <div>
      Dette er <b>Side A</b>.
      <router-link to="/sideb">Gå til Side B</router-link>
  </div>
</template>

<script>
export default {
  name: 'Side A'
}
</script>
```
Eksempel 26 i kapittel 17 - SPA-rammeverket Vue.js
```html
<template>
  <div>
      Dette er <b>Side B</b>.
      <router-link to="/sidea">Gå til Side A</router-link>
  </div>
</template>

<script>
export default {
  name: 'Side B'
}
</script>
```
Eksempel 27 i kapittel 17 - SPA-rammeverket Vue.js
```js
import Vue from 'vue'
import Router from 'vue-router'
import HelloWorld from '@/components/HelloWorld'
import SideA from '@/components/SideA'
import SideB from '@/components/SideB'

Vue.use(Router)

export default new Router({
  routes: [
    {
      path: '/',
      name: 'HelloWorld',
      component: HelloWorld
    },
    {
      path: '/sidea',
      name: 'Side A',
      component: SideA
    },
    {
      path: '/sideb',
      name: 'Side B',
      component: SideB
    },
  ]
})
```
Eksempel 28 i kapittel 17 - SPA-rammeverket Vue.js
```html

<template>
  <div id="app">
    <router-view :personprop="person" @datachanged="handleDatachanged"/>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      person: {
        name: "Terje",
        birthYear: 1975
      }
    };
  },
  methods: {
    handleDatachanged(personData) {
      this.person.name = personData.name;
      this.person.birthYear = personData.birthYear;
    }
  }
};
</script>
```
Eksempel 29 i kapittel 17 - SPA-rammeverket Vue.js
```js
export default new Router({
  routes: [
    {
      path: '/sidea',
      name: 'Side A',
      component: SideA,
      props: true
    },
    {
      path: '/sideb',
      name: 'Side B',
      component: SideB,
      props: true
    }
  ]
})
```
Eksempel 30 i kapittel 17 - SPA-rammeverket Vue.js
```html
<template>
  <div>
    Dette er komponent A<br/>
    <input type="text" v-model="persondata.name" placeholder="Navn"><br/>
    <input type="text" v-model="persondata.birthYear" placeholder="Fødelsesår"><br/>
    <button @click="nav">Til komponent B</button>
  </div>
</template>

<script>
export default {
  name: "CompA",
  props: ["personprop"],
  data() {
    return {
      persondata: {
        name: null,
        birthYear: null
      }
    };
  },
  created() {
    this.persondata.name = this.personprop.name;
    this.persondata.birthYear = this.personprop.birthYear;
  },
  methods: {
    nav() {
      this.$emit("datachanged", this.persondata);
      this.$router.push("/sideb");
    }
  }
};
</script>
```
Eksempel 31 i kapittel 17 - SPA-rammeverket Vue.js
```html
<template>
  <div class="innhold" id="innhold">
    <p v-for="(trekning, i) in trekninger">
      <small>
        {{dagsNavn[new Date(trekning.tid).getDay()]}}
        {{lagDatoTekstForVisning(new Date(trekning.tid))}}
      </small>
      <br>
      <b :class="'førsteTrekning' + i ">
        {{trekning.vinnere.length === 1 ? 'Vinneren' : 'Vinnerne'}}
        er {{lagTekstListe(trekning.vinnere)}}!
      </b>
      <br>
      <small>
        Trukket fra totalt {{trekning.deltakere.length}} personer:
        {{lagTekstListe(trekning.deltakere)}}
      </small>
    </p>
  </div>
</template>

<script>
export default {
  name: "TrekningListe",
  props: ["trekningerProp"],
  data() {
    return {
      trekninger: [],
      dagsNavn: [
        "søndag",
        "mandag",
        "tirsdag",
        "onsdag",
        "torsdag",
        "fredag",
        "lørdag"
      ]
    };
  },
  created() {
    for (let t of this.trekningerProp) {
      this.trekninger.push(t);
    }
  },
  methods: {
    lagDatoTekstForVisning(dato) {
      return dato
        .toLocaleString()
        .replace(",", "")
        .substr(0, 15);
    },
    lagTekstListe(liste) {
      if (liste.length === 0) return "";
      if (liste.length === 1) return liste[0];

      const tekstListe = liste.join(", ");
      const indexSisteKomma = tekstListe.lastIndexOf(",");
      return (
        tekstListe.substr(0, indexSisteKomma) +
        " og " +
        tekstListe.substr(indexSisteKomma + 1)
      );
    }
  }
};
</script>
```
Eksempel 32 i kapittel 17 - SPA-rammeverket Vue.js
```html
<template>
  <div class="innhold" id="innhold">
    <table>
      <tr>
        <td>
          <input type="checkbox" v-model="velgAlle" @click="velgAlleEllerIngen">
        </td>
        <td>
          <b>Personer</b>
        </td>
        <td></td>
      </tr>
      <tr v-for="person in liste">
        <td>
          <input type="checkbox" v-model="person.erValgt">
        </td>
        <td>{{person.navn}}</td>
        <td>
          <button class="litenKnapp" @click="slettPerson(person.id)">x</button>
        </td>
      </tr>
      <tr>
        <td></td>
        <td colspan="3">
          <input size="6" type="text" v-model="nyPerson">
          <button class="litenKnapp" @click="leggTilPerson">legg til person</button>
        </td>
      </tr>
      <tr>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td colspan="3">
          <button class="knapp" @click="trekk">Trekk!</button>
          <input type="number" size="1" v-model="trekkAntall">
          <button class @click="trekkAntall++">▲</button>
          <button class @click="trekkAntall = Math.max(1,personer.trekkAntall -1)">▼</button>
        </td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "PersonListe",
  data() {
    return {
      nyPerson: "",
      velgAlle: false,
      trekkAntall: 1,
      liste: []
    };
  },
  props: ["personerProp"],
  created() {
    for (let p of this.personerProp) {
      this.liste.push(p);
    }
  },
  methods: {
    velgAlleEllerIngen() {
      let verdi = !this.velgAlle;
      for (let person of this.liste) {
        person.erValgt = verdi;
      }
    },
    slettPerson(id) {
      let index = this.liste.findIndex(p => p.id === id);
      if (index == -1) return;
      this.liste.splice(index, 1);
      this.$emit("oppdatert-personliste", this.liste);
    },
    leggTilPerson() {
      const id =
        this.liste
          .map(p => p.id)
          .reduce((max, value) => Math.max(max, value), -1) + 1;
      this.liste.push({ id: id, navn: this.nyPerson, erValgt: true });
      this.nyPerson = "";
      this.$emit("oppdatert-personliste", this.liste);
    },
    trekk() {
      this.$emit("trekk", this.trekkAntall);
    }
  }
};
</script>
```
Eksempel 33 i kapittel 17 - SPA-rammeverket Vue.js
```js
import Vue from 'vue'
import Router from 'vue-router'
import PersonListe from '@/components/PersonListe'
import TrekningListe from '@/components/TrekningListe'

Vue.use(Router)

export default new Router({
  routes: [
    {
      path: '/',
      name: 'PersonListe',
      component: PersonListe,
      props: true
    },
    {
      path: '/trekninger',
      name: 'TrekningListe',
      component: TrekningListe,
      props: true
    }
  ]
})
```
## 18 - Rest-API
Eksempel 1 i kapittel 18 - Rest-API
```js
{
  "categories": [
    
  ],
  "created_at": "2016-05-01 10:51:41.584544",
  "icon_url": "https:\/\/assets.chucknorris.host\/img\/avatar\/chuck-norris.png",
  "id": "ia_mw_KNSV27_MrreHYLVQ",
  "updated_at": "2016-05-01 10:51:41.584544",
  "url": "https:\/\/api.chucknorris.io\/jokes\/ia_mw_KNSV27_MrreHYLVQ",
  "value": "Chuck Norris jumped to the top of Mount Everest."
}
```
Eksempel 2 i kapittel 18 - Rest-API
```html
<head>
    <script src="https://unpkg.com/axios/dist/axios.min.js"></script>
</head>
<body>
    <button onclick="hentData()">Hent vits</button><div id="vits"></div>
    <script>
        let vitsDiv = document.getElementById('vits');

        async function hentData() {
            let resultat = await axios.get('https://api.chucknorris.io/jokes/random');
            let vits = resultat.data;
            console.log(vits);
            vitsDiv.innerHTML = vits.value;
        }
    </script>
</body>
```
## Sende med data
Eksempel 1 i kapittel Sende med data
```js
async function testPost() {
    let files = {
        files: {
            "index.html": { content: "<h1>Hallo</h1>", isBinary: false },
            "index.js": { content: "console.log('hello!')", isBinary: false },
            "package.json": { content: { dependencies: {} } }
        }
    }

    let url = 'https://codesandbox.io/api/v1/sandboxes/define?json=1';
    let resultat = await axios.post(url, files);
    let sandboxId = resultat.data.sandbox_id;
}
```
## 19 - Kodegenerering og metadata
Eksempel 1 i kapittel 19 - Kodegenerering og metadata
```
https://api.chucknorris.io/jokes/random
https://api.chucknorris.io/jokes/random?category={category}
https://api.chucknorris.io/jokes/categories
https://api.chucknorris.io/jokes/search?query={query}
```
Eksempel 2 i kapittel 19 - Kodegenerering og metadata
```js
let urler = [
    'https://api.chucknorris.io/jokes/random',
    'https://api.chucknorris.io/jokes/random?category={category}',
    'https://api.chucknorris.io/jokes/categories',
    'https://api.chucknorris.io/jokes/search?query={query}'
];

kjørTest();

async function kjørTest() {
    let javascriptKode = lagFunksjoner(urler);
    console.log(javascriptKode);
    eval(javascriptKode);
    let tilfeldigVits = await random();
    let tilfeldigFilmvits = await random2('movie');
    let kategorier = await categories();
    let programmeringsvitser = await search2('programming');
    console.log(tilfeldigVits, tilfeldigFilmvits, kategorier, programmeringsvitser;
}
```
Eksempel 3 i kapittel 19 - Kodegenerering og metadata
```js
function lagFunksjoner(urler) {
    let kode = '';
    for (let url of urler) {
        let { navn, param } = analyserUrl(url);
        kode += `async function ${navn}(${param || ''}) {
                     let url = '${url}';
                     url = url.split('?')[0]${param ? ` + '?${param}=' + ${param}` : ''};
                     let resultat = await axios.get(url);
                     return resultat.data;
                 }
        `;
    }
    return kode;
}

function analyserUrl(url) {
    let deler = url.split('/');
    let navn = deler[4];
    let param = null;
    if (navn.includes('?')) {
        let deler2 = navn.split('?');
        navn = deler2[0] + '2';
        param = deler2[1].split('=')[0];
    }
    return { navn, param };
}
```
Eksempel 4 i kapittel 19 - Kodegenerering og metadata
```js
async function random() {
    let url = 'https://api.chucknorris.io/jokes/random';
    url = url.split('?')[0];
    let resultat = await axios.get(url);
    return resultat.data;
}
async function random2(category) {
    let url = 'https://api.chucknorris.io/jokes/random?category={category}';
    url = url.split('?')[0] + '?category=' + category;
    let resultat = await axios.get(url);
    return resultat.data;
}
async function categories() {
    let url = 'https://api.chucknorris.io/jokes/categories';
    url = url.split('?')[0];
    let resultat = await axios.get(url);
    return resultat.data;
}
async function search2(query) {
    let url = 'https://api.chucknorris.io/jokes/search?query={query}';
    url = url.split('?')[0] + '?query=' + query;
    let resultat = await axios.get(url);
    return resultat.data;
}
```
Eksempel 5 i kapittel 19 - Kodegenerering og metadata
```js
random = async () => await chuckNorrisRestKall('random', {} ); 
randomCategory = async (category) => await chuckNorrisRestKall('random', {category} ); 
categories = async () => await chuckNorrisRestKall('categories', {} ); 
searchQuery = async (query) => await chuckNorrisRestKall('search', {query} );
```
Eksempel 6 i kapittel 19 - Kodegenerering og metadata
```js
function lagFunksjoner(urler) {
    let kode = '';
    for (let url of urler) {
        let { navn, param } = analyserUrl(url);
        let funksjonsNavn = navn;
        if (param) funksjonsNavn += param[0].toUpperCase() + param.substr(1);
        kode += `${funksjonsNavn} = async (${param || ''}) => await chuckNorrisRestKall('${navn}', {${param || ''} });`;
    }
    return kode;
}

async function chuckNorrisRestKall(funksjonsnavn, parameterObjekt) {
    let basisUrl = 'https://api.chucknorris.io/jokes/';
    let parametre = '';
    for (let feltNavn in parameterObjekt) {
        let feltVerdi = parameterObjekt[feltNavn];
        let skilletegn = parametre == '' ? '?' : '&';
        parametre += skilletegn + feltNavn + '=' + feltVerdi;
    }
    let url = basisUrl + funksjonsnavn + parametre;
    let resultat = await axios.get(url);
    return resultat.data;
}

function analyserUrl(url) {
    let deler = url.split('/');
    let navn = deler[4];
    let param = null;
    if (navn.includes('?')) {
        let deler2 = navn.split('?');
        navn = deler2[0];
        param = deler2[1].split('=')[0];
    }
    return { navn, param };
}
```
Eksempel 7 i kapittel 19 - Kodegenerering og metadata
```js
let urler = [
    'https://api.chucknorris.io/jokes/random',
    'https://api.chucknorris.io/jokes/random?category={category}',
    'https://api.chucknorris.io/jokes/categories',
    'https://api.chucknorris.io/jokes/search?query={query}'
];
```
Eksempel 8 i kapittel 19 - Kodegenerering og metadata
```js
let chuckNorrisApiMetadata = {
    basisUrl: 'https://api.chucknorris.io/jokes/random',
    tjenester: [
        { navn: 'random', parametre: [] },
        { navn: 'random', parametre: ['category'] },
        { navn: 'categories', parametre: [] },
        { navn: 'search', parametre: ['query'] }
    ]
};
``` 
Eksempel 9 i kapittel 19 - Kodegenerering og metadata
```js
{
    rom: [
        { navn: 'A', innhold: ['rød nøkkel'], start: true },
        { navn: 'B', innhold: ['grønn nøkkel'] },
        { navn: 'C', innhold: ['hvit nøkkel'] },
        { navn: 'D', innhold: ['blå nøkkel'] },
        { navn: 'E', innhold: ['grå nøkkel'] },
        { navn: 'F', innhold: [], vunnet: true },
    ],
    dører: [
        { A: 'B', B: 'A', farge: 'rød', åpen: false },
        { A: 'D', D: 'A', farge: 'grønn', åpen: false },
        { B: 'C', C: 'B', farge: 'grå', åpen: false },
        { B: 'E', E: 'B', farge: 'blå', åpen: false },
        { E: 'F', F: 'E', farge: 'hvit', åpen: false },
    ]
};
```
Eksempel 10 i kapittel 19 - Kodegenerering og metadata
```html
<div id="game">
    <h3 v-if="spiller.rom.vunnet">Gratulerer - du har fullført spillet! :-)</h3>
    <h3 v-else>Du er i rom {{spiller.rom.navn}}</h3>
    <p>
        I rommet ser du:
        <template v-if="spiller.rom.innhold.length == 0">
            <i>ingenting</i>
        </template>
        <template v-else>
            <ul v-for="ting in spiller.rom.innhold">
                <li>{{ting}} <button @click="plukkOpp(ting)">Plukk opp</button></li>
            </ul>
        </template>
    </p><p>
        Du har:
        <template v-if="spiller.har.length == 0">
            <i>ingenting</i>
        </template>
        <template v-else>
            <ul v-for="ting in spiller.har">
                <li>{{ting}}</li>
            </ul>
        </template>
    </p><p>
        Dører:
        <ul v-for="(dør,i) in dørerHer">
            <li>
                {{dør.farge}} dør til rom {{dør.til}}
                <button v-if="dør.åpen" @click="gåTil(dør.til)">Gå gjennom</button>
                <button v-else-if="kanÅpne(dør)" @click="låseOpp(dør.farge)">Låse opp</button>
            </li>
        </ul>
    </p>
</div>
```
Eksempel 11 i kapittel 19 - Kodegenerering og metadata
```js
var app = new Vue({
    el: '#game',
    data: {
        spiller: {
            rom: null,
            har: []
        },
        metadata: { /* som vist over */ }
    },
    computed: {
        dørerHer() {
            let rom = this.spiller.rom.navn;
            return this.metadata.dører.filter(d => d.hasOwnProperty(rom))
                .map(d => {
                    return { farge: d.farge, til: d[rom], åpen: d.åpen }
                });
        }
    },
    created() {
        this.spiller.rom = this.metadata.rom.filter(r => r.start)[0];
    },
    methods: {
        kanÅpne(dør) {
            return this.spiller.har.includes(dør.farge + ' nøkkel');
        },
        plukkOpp(ting) {
            this.spiller.har.push(ting);
            this.spiller.rom.innhold = this.spiller.rom.innhold.filter(t => t != ting);
        },
        låseOpp(dørFarge) {
            let dør = this.metadata.dører.filter(d => d.farge == dørFarge)[0];
            dør.åpen = true;
        },
        gåTil(rom) {
            this.spiller.rom = this.metadata.rom.filter(r => r.navn === rom)[0];
        }
    }
});
```
Eksempel 12 i kapittel 19 - Kodegenerering og metadata
```html
<table style="text-align: left">
  <tr>
    <th>Navn</th>
    <td>Terje Kolderup</td>
  </tr>
  <tr>
    <th>Fødselsår</th>
    <td>1975</td>
  </tr>
</table>
```
Eksempel 13 i kapittel 19 - Kodegenerering og metadata
```html
<template>
  <div>
    <table>
      <tr>
        <th>Navn</th>
        <td>{{person.navn}}</td>
      </tr>
      <tr>
        <th>Fødselsår</th>
        <td>{{person.fødselsår}}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "SkjemaVisning",
  props: ["person"],
  data() {
    return {};
  }
};
</script>

<style scoped>
table {
  text-align: left;
}
</style>
```
Eksempel 14 i kapittel 19 - Kodegenerering og metadata
```html
<skjema-visning :person="{navn: 'Terje Kolderup', fødselsår: 1975}"></skjema-visning>
```		
Eksempel 15 i kapittel 19 - Kodegenerering og metadata
```html
<template>
  <div>
    <h3>{{ metadata.overskrift }}</h3>
    <table>
      <tr v-for="felt in metadata.felt">
        <th>{{ felt.visningsnavn }}</th>
        <td>{{ data[felt.navn] }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "SkjemaVisning",
  props: ["data", "metadata"],
  data() {
    return {};
  }
};
</script>
```
Eksempel 16 i kapittel 19 - Kodegenerering og metadata
```html
<template>
  <div class="hello">
    <skjema-visning :data="person" :metadata="metadata" ></skjema-visning>
  </div>
</template>

<script>
import SkjemaVisning from './SkjemaVisning';

export default {
  name: 'HelloWorld',
  data () {
    return {
      person: {navn: 'Terje Kolderup', fødselsår: 1975},
      metadata: {
        overskrift: 'Hovedperson',
        felt: [
          { visningsnavn: 'Navn', navn: 'navn' },
          { visningsnavn: 'Fødselsår', navn: 'fødselsår' },
        ]
      }
    }
  },
  components: {SkjemaVisning}
}
</script>
```
Eksempel 17 i kapittel 19 - Kodegenerering og metadata
```js
let komponenter = {
    overskrift(data) {},
    skjemaVisning(data, metadata, index) {},
    listeVisning(data, metadata) {},
    meny(data, metadata) {},
};
```
Eksempel 18 i kapittel 19 - Kodegenerering og metadata
```js
overskrift(data) {
    let p = data.tekst ? `<p>${data.tekst}</p>` : '';
    return `<div class="sideElement" style="grid-area: overskrift">
                <h3>${data.overskrift}</h3>
                ${p}
            </div>`;
}
```
Eksempel 19 i kapittel 19 - Kodegenerering og metadata
```js
meny(data, metadata) {
    return `<div class="sideElement" style="grid-area: meny" class="meny">
                <h3>Meny</h3>
                <ul>
                    ${ Object.keys(metadata)
                    .filter(navn => metadata[navn].visningsnavn)
                    .map(navn =>
                            `<li>
                                <a href="javascript:app.visSide('${navn}')">${metadata[navn].visningsnavn}</a>
                             </li>`).join('')}
                </ul>
            </div>`;
}
```
Eksempel 20 i kapittel 19 - Kodegenerering og metadata
```js
sider: {
    forside: {
        visningsnavn: 'Hjem',
    },
    kategoriListe: {
        visningsnavn: 'Kategorier',
    },
    produktListe: {
        visningsnavn: 'Alle produkter',
    },
    enkeltProdukt: {
    },
    kontaktOss: {
        visningsnavn: 'Kontakt oss',
    }
```
Eksempel 21 i kapittel 19 - Kodegenerering og metadata
```js
skjemaVisning(data, metadata, index) {
    if (index != null) {
        data = data[index];
    }
    return `<div class="sideElement" style="grid-area: skjemaVisning">
                <table style="text-align: left">
                    ${ metadata.felt.map(f =>
                    `<tr>
                        <th>${ f.visningsnavn}</th>
                        <td>${ data[f.navn]}</td>
                     </tr>` ).join('')}
                </table></div>`;
}
```
Eksempel 22 i kapittel 19 - Kodegenerering og metadata
```js
listeVisning(data, metadata) {
    return `<div class="sideElement" style="grid-area: listeVisning">
                <table>
                    <tr>
                        ${ metadata.felt.map(f => `<th>${f.visningsnavn}</th>`).join('')}
                    </tr>
                    ${data.map((rad, index) => `
                        <tr>
                            ${ metadata.felt.map(f => `<td>${rad[f.navn]}</td>`).join('')}
                            ${ (metadata.operasjoner || []).map((o) => `
                            <td><a href="javascript:app.visSide('${o.side}', ${index})">${o.tekst}</a></td>`).join('')}
                        </tr>`).join('')}
                </table>
            </div>`;
}
```

Eksempel 23 i kapittel 19 - Kodegenerering og metadata
```js
${ metadata.felt.map(f => `<td>${rad[f.navn]}</td>`).join('')}
```
Eksempel 24 i kapittel 19 - Kodegenerering og metadata
```js
class ProduktkatalogApp {
    constructor() {
        this.data = {
            produkter: [],
            tekster: {}
        };
        this.metadata = {
            produkt: {},
            forside: {},
            kontaktOss: {},
            sider: {},
            maler: {}
        };
    }

    visSide(sidenavn, parameter) {
    }

    renderKomponent(komponentNavn, metadataSide, parameter) {
    }
}

let app = new ProduktkatalogApp();
app.visSide('forside');
```
Eksempel 25 i kapittel 19 - Kodegenerering og metadata
```js
[
    { navn: "Gullskje 22 cm", pris: 990, kategori: "skje" },
    { navn: "Sølvskje 22 cm", pris: 190, kategori: "skje" },
    { navn: "Stålskje 22 cm", pris: 19, kategori: "skje" },
    { navn: "Gullkniv 22 cm", pris: 990, kategori: "kniv" },
    { navn: "Sølvkniv 22 cm", pris: 190, kategori: "kniv" },
    { navn: "Stålkniv 22 cm", pris: 19, kategori: "kniv" },
    { navn: "Gullgaffel 22 cm", pris: 990, kategori: "gaffel" },
    { navn: "Sølvgaffel 22 cm", pris: 190, kategori: "gaffel" },
    { navn: "Stålgaffel 22 cm", pris: 19, kategori: "gaffel" }
]
```
Eksempel 26 i kapittel 19 - Kodegenerering og metadata
```js
tekster: {
    forside: {
        overskrift: "Bestikkshoppen",
        tekst: "Velkommen til Bestikkshoppen AS. Vi håper du får mange flotte handleopplevelser!",
    },
    info: {
        telefon: '987 65 432',
        slagord: 'Vi bestikker deg!'
    },
    produkt: {
        overskrift: "Produkt",
        tekst: "Se detaljer om dette produktet under:"
    },
    produkter: {
        overskrift: "Produkter",
        tekst: "Se våre flotte produkter:"
    },
    kontaktOss: {
        overskrift: "Bestikkshoppen",
        tekst: "Vi gleder oss til å høre fra deg!",
        felt: {
            navn: "Bestikkshoppen AS",
            adresse: "Melkeveien 1",
            postnr: "0123",
            poststed: "Oslo",
            epost: "post@bestikkshoppen.no",
            web: "www.bestikkshoppen.no"
        }
    }
}
```
Eksempel 27 i kapittel 19 - Kodegenerering og metadata
```js
produkt: {
    felt: [
        { navn: 'navn', visningsnavn: 'Navn' },
        { navn: 'pris', visningsnavn: 'Pris', type: 'kroner' },
        { navn: 'kategori', visningsnavn: 'Kategori' },
    ],
    operasjoner: [{ side: 'enkeltProdukt', tekst: 'detaljer' }]
},
forside: {
    felt: [
        { navn: 'telefon', visningsnavn: 'Telefon' },
        { navn: 'slagord', visningsnavn: 'Slagord' },
    ]
},
kontaktOss: {
    felt: [
        { navn: 'navn', visningsnavn: 'Navn' },
        { navn: 'adresse', visningsnavn: 'Adresse' },
        { navn: 'postnr', visningsnavn: 'Postnr.' },
        { navn: 'poststed', visningsnavn: 'Poststed' },
        { navn: 'epost', visningsnavn: 'E-post' },
        { navn: 'web', visningsnavn: 'Web' },
    ]
}
```
Eksempel 28 i kapittel 19 - Kodegenerering og metadata
```js
maler: {
    infoSide: {
        komponenter: ["meny", "overskrift", "skjemaVisning"],
        layout: {
            rader: "200px auto",
            kolonner: "200px auto",
            mal: ["meny overskrift", "meny skjemaVisning"]
        }
    },
    listeSide: {
        komponenter: ["meny", "overskrift", "listeVisning"],
        layout: {
            rader: "200px auto",
            kolonner: "200px auto",
            mal: ["meny overskrift", "meny listeVisning"]
        }
    }
}
```
Eksempel 29 i kapittel 19 - Kodegenerering og metadata
```js
sider: {
    forside: {
        visningsnavn: 'Hjem',
        mal: "infoSide",
        data: { overskrift: "tekster.forside", skjemaVisning: "tekster.info" },
        metadata: { skjemaVisning: "forside", meny: "sider" },
    },
    kategoriListe: {
        visningsnavn: 'Kategorier',
        mal: "listeSide",
        data: { overskrift: "tekster.kategorier", listeVisning: "kategorier" },
        metadata: { meny: "sider", listeVisning: "kategorier" },
    },
    produktListe: {
        visningsnavn: 'Alle produkter',
        mal: "listeSide",
        data: { overskrift: "tekster.produkter", listeVisning: "produkter" },
        metadata: { listeVisning: "produkt", meny: "sider" }
    },
    enkeltProdukt: {
        mal: "infoSide",
        data: { overskrift: "tekster.produkt", skjemaVisning: "produkter" },
        metadata: { skjemaVisning: "produkt", meny: "sider" }
    },
    kontaktOss: {
        visningsnavn: 'Kontakt oss',
        mal: "infoSide",
        data: { overskrift: "tekster.kontaktOss", skjemaVisning: "tekster.kontaktOss.felt" },
        metadata: { skjemaVisning: "kontaktOss", meny: "sider" }
    }
}
```
Eksempel 30 i kapittel 19 - Kodegenerering og metadata
```js
visSide(sidenavn, parameter) {
    let metadataSide = this.metadata.sider[sidenavn];
    let metadataMal = this.metadata.maler[metadataSide.mal];
    let style = `
        grid-template-rows: ${metadataMal.layout.rader};
        grid-template-columns: ${metadataMal.layout.kolonner};
        grid-template-areas: '${metadataMal.layout.mal.join(`' '`)}';
        `;
    let innhold = metadataMal.komponenter.map(k => 
        this.renderKomponent(k, metadataSide, parameter)).join('');
    document.getElementById('side').outerHTML =
        `<div class="innhold" id="side" style="${style}">
            <!-- ${sidenavn} -->
            ${innhold}
            </div>`;
}
```
Eksempel 31 i kapittel 19 - Kodegenerering og metadata
```js
renderKomponent(komponentNavn, metadataSide, parameter) {
    let komponentFunksjon = komponenter[komponentNavn];
    if (!komponentFunksjon) console.log('mangler komponent: ' + komponentNavn);
    let dataSti = (metadataSide.data || {})[komponentNavn] || '';
    let metadataSti = (metadataSide.metadata || {})[komponentNavn] || '';
    return `<!-- start ${komponentNavn} --> 
                ${komponentFunksjon(
                    this.hentVerdi(dataSti, this.data),
                    this.hentVerdi(metadataSti, this.metadata), parameter)}
            <!-- slutt ${komponentNavn} --> `;
}

hentVerdi(sti, objekt) {
    for (let feltNavn of sti.split('.')) {
        objekt = objekt[feltNavn];
    }
    return objekt;
}
```
