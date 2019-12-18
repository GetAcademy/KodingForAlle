## Forord
## Innhold
## 1 - HTML
1
```html
<h1>Min første web-side</h1>
```
2
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
3
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
4
```html
☰ Vinlotterix<br/>
<small>onsdag 17.10.18</small><br/>
<b>Vinneren er Ole!</b><br/>
<small>Trukket fra totalt 3 personer: Per, Pål og Ole</small>
```
5
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
1
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
2
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
3
```css
div.specialEffect {
  border: 4px dashed orange;
  padding: 5px;
}
```
4
```html
<div>A</div>
<div class="specialEffect">B</div>
<div>C</div>
```
5
```html
<div class="specialEffect">B</div>
``` 
## Vinlotterix - Prototyping 2 - CSS
1
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
2
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
1
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
2
```html
<div class="page" style="display: grid; background-color: lightblue">
```
3
```css
div.page {
    display: grid;
}
```
4
```css
div.page {
    height: 100vh;
    display: grid;
    grid-template-columns: 2fr 1fr 3fr;
}
```
5
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
1
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
2
```css
    grid-template-areas: 'header header' 
                         'innhold innhold';
```
3
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
1
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
1
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
1
```html
<script>
    alert('Hei på deg!');
</script>
```
2
```html
<h1 onclick="alert('Takk :-)');">Trykk på meg!</h1>
``` 
3
```js
alert('Hei');
alert('på');
alert('deg!');
```
4
```js
function heiPåDeg() {
    alert('Hei');
    alert('på');
    alert('deg!');
}
```
5
```html
<h1 id="overskrift" onclick="endreTekst()">Trykk på meg!</h1>
<script>
    function endreTekst() {
        document.getElementById('overskrift').innerHTML = 'Takk :-)';
    }
</script>
```
6
```html
<h1 onclick="endreTekst()">Trykk på meg for å endre overskriften under!</h1>
<h1 id="overskrift" >Trykk på overskriften over for å endre meg!</h1>
<script>
    function endreTekst() {
        document.getElementById('overskrift').innerHTML = 'Takk :-)';
    }
</script>
```
7
```html
<b id="overskrift" onclick="endreTekst()">Trykk for prikker:</b>
<script>
    function endreTekst() {
        document.getElementById('overskrift').innerHTML += ' •';
    }
</script>
```
8
```html
<div id="minDiv" style="background-color: red;">Hei</div>
```
9
```js
document.getElementById('minDiv').style.backgroundColor = 'red';
```
10
```css
div.rødOgFin {
    background-color: red;
}
```
11
```js
document.getElementById('minDiv').classList.add('rødOgFin');
```
12
```js
document.getElementById('minDiv').classList.remove('rødOgFin');
```
13
```html
<div id="innhold">
    Jeg tenker på et tall mellom 1 og 20. Tipp hvilket!<br />
    <input type="text" /> <button onclick="tipp1()">Tipp</button>
</div>
```
14
```js
function tipp1() {
    document.getElementById('innhold').innerHTML = `
            Du tippet 27. Det er for høyt - tipp igjen!<br/>
            <input type="text"/><button onclick="tipp2()">Tipp</button>
            `;
}
```
15
```js
function tipp2() {
    document.getElementById('innhold').innerHTML = `
            Du tippet 12 - og det er riktig! 😀<br/>
            <button onclick="tipp2()">Start på nytt</button>
            `;
}
```
16
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
17
```js
function visOgSkjulMeny() {
    document.getElementById('page').classList.toggle('pageUtenMeny');
}
```
18
```css
div.pageUtenMeny {
    grid-template-columns: 0px 2fr;
}
```
19
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
20
```html
<button onclick="alert(this.innerHTML)">Hei!</button>
<button onclick="alert(this.innerHTML)">Hallo!</button>
```
21
```html
<button onclick="this.innerHTML = 'x'">Hei!</button>
<button onclick="this.innerHTML = 'x'">Hallo!</button>
```
22
```html
<h1 onclick="trykk(this)">Trykk!</h1>
<h1 onclick="trykk(this)">Trykk!</h1>
<script>
    function trykk(trykketPåTag) {
        trykketPåTag.innerHTML = 'x';
    }
</script>
```
23
```html
<h1 onclick="trykk()">Trykk!</h1>
<h1 id="o">Trykk!</h1>
<script>
    function trykk() {
        document
          .getElementById('o')
          .innerHTML = 'x';
    }
</script>
```
24
```js
document.getElementById('o').innerHTML = 'x';
```
25
```js
alert('Hei' + 'på' + 'deg!');
```
26
```html
<button onclick="alert('Hei, ' + this.innerHTML + '!')">Per</button>
<button onclick="alert('Hei, ' + this.innerHTML + '!')">Pål</button>
<button onclick="alert('Hei, ' + this.innerHTML + '!')">Espen</button>
```
27
```js
var tekst = 'Hei, ' + navn + '. Hvordan står det til i ' + sted + '?';
```
28
```js
var tekst = `Hei, ${navn}. Hvordan står det til i ${sted}?`;
```
29
```js
var tekst = `Hei, ${navn}. 
             Hvordan står det til i ${sted}?`;
```
30
```js
var tekst = 'Hei, ' + navn + '.' 
          + 'Hvordan står det til i ' + sted + '?';
```
31
```html
<script>
    console.log('Hei');
    console.log('på');
    console.log('deg!');
</script>
```
32
```js
var navnFraSkjema = document.getElementById('navn').value;
```
33
```js
var minDiv = document.getElementById('minDiv');
minDiv.style.backgroundColor = '#4567ab';
minDiv.style.color = '#4567ab';
minDiv.style.padding = '4px';
minDiv.classList.add('active');
minDiv.classList.remove('old');
minDiv.classList.toggle('something');
```
34
```html
<div class="something old"></div>
```
35
```html
<div class="active"></div>
```
36
```html
<input type="text"
       onclick="console.log('onclick ' + this.value)"
       oninput="console.log('oninput ' + this.value)"
       onchange="console.log('onchange ' + this.value)"/>
```
37
```
onclick 
oninput h
oninput he
oninput hei
onchange hei
```
## 5 - Variabler
1
```js
var teller;
```
2
```js
teller = 0;
```
3
```js
var tall = 123;
```
4
```js
a = 5;
b = a;
```
5
```js
a = 5;
b = a;
a = 6;
a = 7;
a = 8;
```
6
```js
var navn = 'Terje';
```
7
```js
var navn = Terje;
```
8
```js
var tekst = 'Hei' + ' på ' + 'deg!';
console.log(tekst);
```
9
```js
var divHtml = document.getElementById('div5').innerHTML;
```
10
```js
document.getElementById('mainContent').innerHTML = 'B!';
``` 
11
```js
var mainContentDiv = document.getElementById('mainContent');
mainContentDiv.innerHTML = 'B!';
``` 
12
```js
var contentTmp = document.getElementById('divA').innerHTML;
document.getElementById('divA').innerHTML = 
    document.getElementById('divB').innerHTML;
document.getElementById('divB').innerHTML = contentTmp;
```
13
```js
var divA = document.getElementById('divA');
var divB = document.getElementById('divB');
var contentTmp = divA.innerHTML;
divA.innerHTML = divB.innerHTML;
divB.innerHTML = contentTmp;
```
14
```html
<div id="content">Hallo!</div>
<button onclick="wrap()">Wrap!</button>
```
15
```js
function wrap() {
    var contentDiv = document.getElementById('content');
    var innhold = contentDiv.innerHTML;
    contentDiv.innerHTML = '<ul><li>' + innhold + '</li><li>'
        + innhold + '</li></ul>';
}
```
16
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
17
```js
var antallKlikk = 0;

function tell() {
    antallKlikk++;
    console.log(antallKlikk);
}
```
18
```html
<button onclick="merk(this)">A</button>
<button onclick="merk(this)">B</button>
<button onclick="merk(this)">C</button>
```
19
```js
function merk(element){
  element.style.border = 'dashed orange 2px';
}
```
20
```js
var forrigeElement;

function merk(element){
  element.style.border = 'dashed orange 2px';
  forrigeElement.style.border = 'none';
  forrigeElement = element;
}
```
21
```html
<button id="knappA" onclick="merk(this)">A</button>
<button onclick="merk(this)">B</button>
<button onclick="merk(this)">C</button>
```
22
```js
var forrigeElement = document.getElementById('knappA');

function merk(element){
  element.style.border = 'dashed orange 2px';
  forrigeElement.style.border = 'none';
  forrigeElement = element;
}
```
23
```js
var tekstA = '5';
var tekstB = '7';
var tallA = parseInt(tekstA);
var tallB = parseInt(tekstB);
var x = tallA + tallB; 
```
24
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
25
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
1
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
2
```js
antallKlikk++;
if( antallKlikk == 10 ) {
    infoDiv.innerHTML = 'Du har klikket 10 ganger.';
}
```
3
```js
antallKlikk++;
if( antallKlikk == 10 ) {
    infoDiv.innerHTML = 'Du har klikket 10 ganger.';
} else {
    infoDiv.innerHTML = '';
}
```
4
```js
antallKlikk++;
infoDiv.innerHTML = '';
if( antallKlikk == 10 ) {
    infoDiv.innerHTML = 'Du har klikket 10 ganger.';
}
```
5
```js
antallKlikk++;
if( antallKlikk < 10 ) {
    infoDiv.innerHTML = 'Du har klikket 9 ganger eller mindre.';
} else {
    infoDiv.innerHTML = 'Du har klikket 10 ganger eller mer.';
}
```
6
```js
antallKlikk++;
if( antallKlikk >= 10 ) {
    infoDiv.innerHTML = 'Du har klikket 10 ganger eller mer.';
} else {
    infoDiv.innerHTML = 'Du har klikket 9 ganger eller mindre.';
}
```
7
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
8
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
9
```js
if(a == 1) x = 10;
else x = 20;
     y = 5;
```
10
```js
if(a == 1) {
    x = 10;
} else {
    x = 20;
    y = 5;
}
```
11
```js
if( navn == 'Terje' ) {
    alert('Terje, jo!');
}
```
12
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
13
```js
if (txt1 == txt2) html += 'Tekst 1 og 2 er like<br/>';
if (txt1 != txt2) html += '<del>Tekst 1 og 2 er like</del><br/>';
```
14
```js
if (txt1 == txt2) html += 'Tekst 1 og 2 er like<br/>';
else html += '<del>Tekst 1 og 2 er like</del><br/>';
```
15
```js
document.getElementById('abc').innerHTML = '<h1>Overskrift</h1>';
```
16
```js
var abcDiv = document.getElementById('abc');
abcDiv.innerHTML = '<h1>Overskrift</h1>';
```
17
```js
var div1 = document.getElementById('aaa');
var div2 = document.getElementById('bbb');
if( div1 == div2 ) {
    ...
}
```
18
```js
var div1 = document.getElementById('aaa');
var div2 = document.getElementById('aaa');
if( div1 == div2 ) {
    ...
}
```
19
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
20
```js
if (txt1 <= txt2) {
    if (txt3 <= txt1) html += txt3;
    else html += txt1;
} else {
    if (txt3 <= txt2) html += txt3;
    else html += txt2;
}
```
21
```js
if( betingelse1 ) {
    if( betingelse2 ) {
        ...
    }
}
```
22
```js
if( betingelse1 & betingelse2 ) {
    ...
}
```
23
```js
if (txt1 <= txt2 & txt1 <= txt3) html += txt1;
else if (txt2 <= txt1 & txt2 <= txt3) html += txt2;
else html += txt3;
```
24
```js
if (txt1 <= txt2 & txt1 <= txt3) html += txt1;
else if (txt2 <= txt3) html += txt2;
else html += txt3;
```
25
```js
if( txt != undefined & txt.length == 10 )
```  
26
```js
if( txt != undefined && txt.length == 10 )
```  
27
```
<br/>A <input type="checkbox"/>
<br/>B <input type="checkbox" checked="checked"/>
```
28
```js
var erValgt = document.getElementById('chk1').checked;
```
29
```js
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
30
```js
var erValgt = document.getElementById('chk1').checked;
if( erValgt ) {
    ...
}
```
31
```js
if( document.getElementById('chk1').checked ) {
    ...
}
```
32
```js
if( n < 10 ) {
    ...
}
```
33
```js
var verdienErRiktig = n < 10;
if( verdienErRiktig ) {
    ...
}
```
34
```js
var a = true;
var b = false;
```
35
```js
if( !document.getElementById('chk1').checked ) {
    ...
}
```
36
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
37
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
38
```js
if ((bunnTykk.checked || bunnTynn.checked) &&
    (fyllTaco.checked || fyllKylling.checked || fyllPepperoni.checked) &&
    (strStor.checked || strMiddels.checked || strLiten.checked)) {
    infoDiv.innerHTML = 'Du har fylt ut alt og er klar til å bestille!';
} 
```
39
```js
if ( bunnTykk.checked || bunnTynn.checked &&
     fyllTaco.checked || fyllKylling.checked || fyllPepperoni.checked &&
     strStor.checked || strMiddels.checked || strLiten.checked ) 
```
40
```js
if ( bunnTykk.checked 
    || bunnTynn.checked && fyllTaco.checked 
    || fyllKylling.checked 
    || fyllPepperoni.checked && strStor.checked 
    || strMiddels.checked 
    || strLiten.checked ) 
```
41
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
1
```js
var popupDiv = document.getElementById('popup');

function visPopup() {
    popupDiv.innerHTML = 'Endringen er lagret. <br/><button onclick="lukkPopup()">Ok</button>';
}

function skulPopup() {
    popupDiv.innerHTML = '';
}
```
2
```js
function visPopup( tekst ) {
    popupDiv.innerHTML = tekst + '<br/><button onclick="lukkPopup()">Ok</button>';
}
```
3
```js
function visLagretPopup() {
    visPopup( 'Endringen er lagret.' );
}
```
4
```html
<button onclick="lukkPopup()">Ok</button>'
```
5
```html
<button onclick="visPopup()">Ok</button>'
```
6
```js
function visPopup( tekst ) {
    if( tekst ) {
        popupDiv.innerHTML = tekst + '<br/><button onclick="lukkPopup()">Ok</button>';
    } else {
        popupDiv.innerHTML = '';
    }
}
```
7
```js
function visPopup( tekst ) {
    popupDiv.innerHTML = tekst ? tekst + '<br/><button onclick="lukkPopup()">Ok</button>' : '';
}
```
8
```js
popupDiv.innerHTML = !tekst ? '' : tekst + '<br/><button onclick="lukkPopup()">Ok</button>';
```
9
```js
var tilfeldigTerningVerdi = Math.ceil( Math.random() * 6 );
```
10
```js
var tilfeldigTerningVerdi1 = Math.ceil( Math.random() * 6 );
var tilfeldigTerningVerdi2 = Math.ceil( Math.random() * 6 );
```
11
```js
function lagTilfeldigTerningverdi() {
    return Math.ceil( Math.random() * 6 ); 
}

var tilfeldigTerningVerdi1 = lagTilfeldigTerningverdi();
var tilfeldigTerningVerdi2 = lagTilfeldigTerningverdi();
```
12
```js
function bestill( antallBilletter ) {
    if( antallBilletter < 1 | antallBilletter > 6 ) return;
    // fortsett med å gjennomføre bestillingen her
}
```
13
```js
function tilfeldigTall(minimum, maksimum) {
    return minimum + Math.floor(Math.random() * (maksimum - minimum + 1));
}
```
14
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
15
```js
function tilfeldigTallEllerBokstavABCDEF() {
    var tall = tilfeldigTall(0, 15);
    if (tall < 10) return tall;
    const charCodeA = 'a'.charCodeAt(0);
    return String.fromCharCode(tall - 10 + charCodeA);
}
```
16
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
17
```js
document.body.style.backgroundColor = tilfeldigFarge();
```
18
```html
<script>
    var a = 5;
</script>
```
19
```js
function telle() {
    var b = 5;
    b++;
    a++;
}
```
20
```js
const minDiv = document.getElementById('divenmin');
```
21
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
1
```js
function snu(tekst) {
    let snuddTekst = '';
    for (let i = tekst.length - 1; i >= 0; i--) {
        snuddTekst += tekst[i];
    }
    return snuddTekst;
}
```
2
```js
function snu(tekst) {
    let snuddTekst = '';
    for (const bokstav of tekst) {
        snuddTekst = bokstav + snuddTekst;
    }
    return snuddTekst;
}
```
3
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
4
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
5
```js
function sorter( tall1, tall2, tall3 ) {
}
```
6
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
7
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
8
```
> liste = ['Per','Pål', 'Espen']
  (3) ["Per", "Pål", "Espen"]
```
9
```
> liste.splice(1)
  (2) ["Pål", "Espen"]
```
10
```
> liste
  ["Per"]
```
## 9 - Model View Controller
1
```html
<div id="smiley" onclick="klikk()"></div>
<div id="poeng"></div>
<button onclick="kjøpOppgradering()">Kjøp oppgradering (10 poeng)</button>
```
2
```html
<style>
    div {
        font-size: 500%;
        user-select: none;
    }
</style>
```
3
```js
// model
var poeng = 0;
var poengPerKlikk = 1;
var visFørsteSmiley = true;
```
4
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
5
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
1
```js
if (confirm('Vil du fortsette?')) {
    alert('Hurra!');
}
```
2
```js
while (confirm('Vil du fortsette?')) {
    alert('Hurra!');
}
```
3
```js
var tall = 1;
while (tall < 10) {
    document.body.innerHTML += tall + ' ';
    tall++;
}
```
4
```js
for (var tall = 1; tall < 10; tall++) {
    document.body.innerHTML += tall + ' ';
}
```
5
```js
for (;confirm('Vil du fortsette?');) {
    alert('Hurra!');
}
```
6
```js
for (var tall = 100; tall < 200; tall += 7) {
    document.body.innerHTML += tall + ' ';
}
```
7
```js
function visTall(førsteTall, sisteTall, endring) {
    for (var tall = førsteTall; tall <= sisteTall; tall += endring) {
        document.body.innerHTML += tall + ' ';
    }
}
```
8
```js
function visTall(tall, antallTall, endring) {
    while (antallTall > 0) {
        document.body.innerHTML += tall + ' ';
        tall += endring;
        antallTall--;
    }
}
```
9
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
1
```js
let navn = ['Per', 'Pål', 'Espen'];
```
2
```js
let navn = [];
navn[0] = 'Per';
navn[1] = 'Pål';
navn[2] = 'Espen';
```
3
```js
var html = '<ul>';
for(let indeks = 0; indeks < navn.length; indeks++) {
    html+= `<li>${navn[indeks]}</li>`;
}
html += '</ul>';
document.getElementById('enId').innerHTML = html;
```
4
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
5
```js
for(let personNavn of alleNavn) {
    html+= `<li>${personNavn}</li>`;
}
```
6
```js
let obj = { a: 1, b: 2, c: 3 };
for (let felt in obj) {
    let verdi = obj[felt];
    console.log(`${felt}=${verdi}`);
}
```
7
```js
liste.splice(3, 1);
```
8
```js
tall.splice(7, 0, 1, 2, 3);
```
9
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
10
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
11
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
12
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
13
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
14
```js
function finnGjennomsnitt(minListe) {
    return finnSum(minListe) / minListe.length;
}
```
15
```js
let liste1 = [1,2,3];
let liste2 = liste1;
liste1[0] = 5;
```
## 12 - Funksjonell programmering
1
```js
function areal(lengde, bredde) {
    return lengde * bredde;
}
```
2
```js
function (lengde, bredde) {
    return lengde * bredde;
}
```
3
```js
let beregnetAreal = function (lengde, bredde) {
                        return lengde * bredde;
                    }(3, 4);
```
4
```js
const areal = function (lengde, bredde) {
    return lengde * bredde;
}
```
5
```js
const areal = (lengde, bredde) => lengde * bredde;
```
6
```js
const kvadrat = side => side * side;
const tilfeldigTerningVerdi = ()) => Math.ceil(Math.random() * 6);
```
7
```js
const html = (tagNavn, innhold) => `<${tagNavn}>${innhold}</${tagNavn}>`;
```
8
```js
const html = tagNavn => innhold => `<${tagNavn}>${innhold}</${tagNavn}>`;
```
9
```js
const h3 = html('h3');
const b = html('b');
```
10
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
11
```js
function filtrerTallOverGrense(minListe, grense) {
    return minListe.filter(tall => tall >= grense);
}
```
12
```js
let alleNavnUpperCase = alleNavn.map(n=>n.toUpperCase());
```
13
```js
let kurs = 8.57;
let beløpNOK = beløpUSD.map(b => b*kurs);
```
14
```js
let tall = [3,7];
let sum = tall.reduce((sum, tall)=>tall+sum, 0);
```
15
```js
let alleNavn = ['Per', 'Pål', 'Espen'];
let html = alleNavn.reduce((htmlListe, navn)=>htmlListe + `<li>${navn}</li>`, '<ul>') + '</ul>';
```
## 13 - Objekter
1
```html
<input type="tall" onkeydown="if (event.code === 'Enter') leggTilTall(this);" />
<div id="statistikk"></div>
```
2
```js
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
```
3
```js
let person = {};
person.navn = 'Terje';
person.by = 'Stavern';
```
4
```js
let person = {
    navn: 'Terje',
    by: 'Stavern',
};
```
5
```js
let navn = 'Terje';
let by = 'Stavern';
let person = {navn, by};
```
6
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
7
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
8
```js
// model
var oppgaver = [
    { beskrivelse: 'Handle til middag', erGjort: true },
    { beskrivelse: 'Lage middag', erGjort: false },
    { beskrivelse: 'Spise middag', erGjort: false },
];
```
9
```html
<table id="oppgaveTabell"></table>
<p>
    <input id="oppgaveBeskrivelse" type="text"/>
    <button onclick="leggTilOppgave()">Legg til oppgave</button>
</p>
```
10
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
11
```js
function endreErGjort(checkbox, indeks) {
    oppgaver[indeks].erGjort = checkbox.checked;
    vis();
}
```
12
```js
function slettOppgave(indeks) {
    oppgaver.splice(indeks, 1);
    vis();
}
```
13
```js
function redigerOppgave(indeks) {
    oppgaver[indeks].redigeringsModus = true;
    vis();
}
```
14
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
15
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
16
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
17
```html
<head>
    <link rel="stylesheet" href="css/vinlotterix.css" />
    <script src="js/model.js"></script>
    <script src="js/common.js"></script>
    <script src="js/personer.js"></script>
    <script src="js/vinnere.js"></script>
</head>
```
18
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
19
```js
visPersoner();

function visOgSkjulMeny() {
    document.getElementById('page').classList.toggle('pageUtenMeny');
}
```
20
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
21
```js
liste.splice(3, 1);
```
22
```js
tall.splice(7, 0, 
    {fornavn: 'Per', etternavn: 'Olsen'},
    {fornavn: 'Pål', etternavn: 'Nilsen'},
    {fornavn: 'Espen', etternavn: 'Hansen'});
```
23
```js
let tall = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
tall.sort()
```
24
```js
tall.sort((a, b) => a === b ? 0 : a < b ? -1 : 1);
```
25
```js
tall.sort((a, b) => a - b);
```
26
```js
tall.sort((a, b) => b - a);
```
27
```js
let personer = [    
    {fornavn: 'Per', etternavn: 'Olsen', alder: 19},
    {fornavn: 'Pål', etternavn: 'Nilsen', alder: 18},
    {fornavn: 'Espen', etternavn: 'Hansen', alder: 17}
];
personer.sort((a, b) => a.alder - b.alder);
```
28
```js
personer.sort(((a,b) => a.etternavn === b.etternavn ? 0 : 
                        a.etternavn < b.etternavn ? 1 : -1);
```
29
```js
personer.sort(((a,b) => a.etternavn.localCompare(b.etternavn));
```
30
```js
personer.sort((a, b) => {
  let step1 = a.etternavn.localeCompare(b.etternavn);
  return step1 != 0 ? step1 : a.fornavn.localeCompare(b.fornavn);
});
```
31
```js
personer.sort((a, b) => a.etternavn.localeCompare(b.etternavn) 
                     || a.fornavn.localeCompare(b.fornavn)});
```
32
```js
let personerUnder18 = personer.filter(p => p.alder < 18);
}
```
33
```js
let hansens = personer.filter(p => p.etternavn === 'Hansen');
}
```
34
```js
let person = personer.filter(p => p.id === 1037)[0];
}
```
35
```js
let listeFulleNavn = personer.map(p => p.fornavn + ' ' + p.etternavn);
}
```
36
```js
let listeAldersverdier = personer.map(p => p.alder);
}
```
37
```js
let sumAvAlder = personer.reduce((sum, p) => p.alder + sum, 0);
```
38
```js
personer.reduce((max, p) => Math.max(p.alder, max), 0);
```
## 14 - Callbacks, promises og asynkrone kall
1
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
2
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
3
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
4
```js
function bestillPizza() {
    lagPizza(pizza => minDiv.innerHTML = pizza);
}

function lagPizza(callback) {
    let html = '<img width="400" src="http://storage.googleapis.com/bro-cdn1/zgrid/themes/10307/images/home/pizza.png"/>';
    callback(html);
}
``` 
5
```html
<button id="minKnapp" onclick="gjørNoe()">Trykk på meg!</button>

<script>
    function gjørNoe() {
        // ...
    }
</script>
```
6
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
7
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
8
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
9
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
10
```js
posisjon(function (posisjon) {
    sted(posisjon, function(sted){
        værvarsel(sted, function (varselet){
            document.getElementById('varsel').innerHTML = varselet;
        })
    });
});
```
11
```js
posisjonPromise()
    .then(posisjon => stedPromise(posisjon))
    .then(sted => værvarselPromise(sted))
    .then(varsel => document.getElementById('varsel').innerHTML = varsel)
    .catch(error => console.error(error));
```
12
```js
function stedPromise(posisjon) {
    return new Promise(function (resolve, reject) {
        sted(posisjon, function (sted) {
            resolve(sted);
        });
    });
}
```
13
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
14
```js
function finnVærvarsel() {
    posisjonPromise()
        .then(posisjon => stedPromise(posisjon))
        .then(sted => værvarselPromise(sted))
        .then(varsel => document.getElementById('varsel').innerHTML = varsel)
}
```
15
```js
async function finnVærvarsel() {
    let posisjon = await posisjonPromise();
    let sted = await stedPromise(posisjon);
    let varsel = await værvarselPromise(sted);
    document.getElementById('varsel').innerHTML = varsel;
}
```
16
```js
function finnVærvarsel() {
    posisjonPromise()
        .then(posisjon => stedPromise(posisjon))
        .then(sted => værvarselPromise(sted))
        .then(varsel => document.getElementById('varsel').innerHTML = varsel)
        .catch(error => console.error(error));
}
```
17
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
18
```js
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
1
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
2
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
3
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
4
```js
let kommentarCollection = db.collection('kommentarer');
let dokumentReferanse = kommentarCollection.doc(id);
unsubscribe = await dokumentReferanse.onSnapshot(
    function (dokumentSnapshot) {
        let dokument = dokumentSnapshot.data();
        console.log(dokument);
    });
```
5
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
6
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
7
```js
async function lesAlleDokumentene() {
    let kommentarCollection = db.collection('kommentarer');
    let collectionSnapshot = await kommentarCollection.get();
    let collection = collectionSnapshot.docs.map(dokumentSnapshot => dokumentSnapshot.data());
}
```
8
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
9
```js
let kommentarCollection = db.collection('kommentarer');
let query = kommentarCollection.where('forfatter', '==', 'Terje')
let collectionSnapshot = await query.get();
```
10
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
11
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
12
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
13
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
1
```js
motor.start();
```
2
```js
let ruteH3 = {
    kolonne: 'H',
    rad: 3
};
```
3
```js
function kode(rute) {
    return rute.kolonne + rute.rad;
}
```
4
```js
class Rute {
    kode() {
        return this.kolonne + this.rad;
    }
}
```
5
```js
let ruteH3 = new Rute();
ruteH3.rad = 3;
ruteH3.kolonne = 'H';
console.log(ruteH3.kode());
```
6
```js
let ruteH3 = {};
ruteH3.rad = 3;
ruteH3.kolonne = 'H';
console.log(kode(ruteH3));
```
7
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
8
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
9
```js
let ruteH3 = new Rute('H', 3);
```
10
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
11
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
12
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
13
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
14
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
        else if (this.type == 'Løper') {
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
15
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
16
```
Program->Brett: flytt('a1', 'a4')
Brett->Brett: finnBrikke('a1')
Brett->Brikke: flyttTilPosisjon('a4')
```
17
```js
flyttTil(kolonne, rad) {
    this.kolonne = kolonne;
    this.rad = rad;
    return true;
}
```
18
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
1
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
2
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
3
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
4
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
5
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
                visOgSkjulMeny: function () {
                    this.showMenu = !this.showMenu;
                },
                lagTekstListe: function (liste) {
                    if (liste.length === 0) return '';
                    if (liste.length === 1) return liste[0];
                    const tekstListe = liste.join(', ');
                    const indexSisteKomma = tekstListe.lastIndexOf(',');
                    return tekstListe.substr(0, indexSisteKomma)
                        + ' og ' + tekstListe.substr(indexSisteKomma + 1);
                },
                lagDatoTekstForVisning: function (dato) {
                    return dato.toLocaleString().replace(',', '').substr(0, 15);
                },
                lagDatoTekstForLagring: function (dato) {
                    return dato.toISOString().substr(0, 16).replace('T', ' ');
                },
                lagDatoTekstNåForLagring: function () {
                    return this.lagDatoTekstForLagring(new Date());
                },
                velgAlleEllerIngen: function () {
                    let verdi = !this.personer.velgAlle;
                    for (let person of this.personer.liste) {
                        person.erValgt = verdi;
                    }
                },
                slettPerson: function (id) {
                    let index = this.personer.liste.findIndex((p => p.id === id));
                    if (index == -1) return;
                    this.personer.liste.splice(index, 1);
                },
                leggTilPerson: function () {
                    const id = this.personer.liste
                        .map(p => p.id).reduce((max, value) => Math.max(max, value), -1) + 1;
                    this.personer.liste
                        .push({ id: id, navn: this.personer.nyPerson, erValgt: true });
                },
                trekk: function () {
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
6
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
7
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
8
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
9
```html
<super-teller start="1000"></super-teller>
<super-teller start="0"></super-teller>
```
10
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
11
```js
Vue.component('person-liste', {
    props: ['personerProp'],
    data: function () {
        return {
            nyPerson: '',
            velgAlle: false,
            trekkAntall: 1,
            liste: []
        };
    },
    created: function () {
        this.liste.push(...this.personerProp);
    },
    methods: {
        velgAlleEllerIngen: function () {
            let verdi = !this.velgAlle;
            for (let person of this.liste) {
                person.erValgt = verdi;
            }
        },
        slettPerson: function (id) {
            let index = this.liste.findIndex((p => p.id === id));
            if (index == -1) return;
            this.liste.splice(index, 1);
            this.$emit('oppdatert-personliste', this.liste);
        },
        leggTilPerson: function () {
            const id = this.liste
                .map(p => p.id).reduce((max, value) => Math.max(max, value), -1) + 1;
            this.liste
                .push({ id: id, navn: this.nyPerson, erValgt: true });
            this.nyPerson = '';
            this.$emit('oppdatert-personliste', this.liste);
        },
        trekk: function () {
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
12
```js
Vue.component('trekning-liste', {
    props: ['trekningerProp'],
    data: function () {
        return {
            trekninger: [],
            dagsNavn: ['søndag', 'mandag', 'tirsdag', 'onsdag', 'torsdag', 'fredag', 'lørdag']
        }
    },
    created: function () {
        this.trekninger.push(...this.trekningerProp);
    },
    methods: {
        lagDatoTekstForVisning: function (dato) {
            return dato.toLocaleString().replace(',', '').substr(0, 15);
        },
        lagTekstListe: function (liste) {
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
13
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
                visOgSkjulMeny: function () {
                    this.showMenu = !this.showMenu;
                },
                lagDatoTekstForLagring: function (dato) {
                    return dato.toISOString().substr(0, 16).replace('T', ' ');
                },
                lagDatoTekstNåForLagring: function () {
                    return this.lagDatoTekstForLagring(new Date());
                },
                trekk: function (antall) {
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
                oppdaterPersoner: function (personer) {
                    this.personer.length = 0;
                    this.personer.push(...personer);
                }
            }
        });
    </script>
</body>
</html>
```
14
```js
tell() {
    this.teller++;
    if(this.teller == this.slutt){
        this.$emit('fullført', this.teller);
    }
}
```
15
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
16
```
npm install -g @vue/cli
npm install -g @vue/cli-init
```
17
```
vue init webpack vuetest
```
18
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
19
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
20
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
21
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
22
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
23
```
DONE  Compiled successfully in 3323ms                             14:55:17
 I  Your application is running here: http://localhost:8080
```
24
```html
<a name="seksjon1"/><p><h1>Seksjon 1</h1>Bla bla bla.<hr style="height: 500px" /></p>
<a name="seksjon2"/><p><h1>Seksjon 2</h1>Bla bla bla.<hr style="height: 500px" /></p>
<a name="seksjon3"/><p><h1>Seksjon 3</h1>Bla bla bla.<hr style="height: 500px" /></p>
```
25
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
26
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
27
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
28
```html

<template>
  <div id="app">
    <router-view :personprop="person" @datachanged="handleDatachanged"/>
  </div>
</template>

<script>
export default {
  name: "App",
  data: function() {
    return {
      person: {
        name: "Terje",
        birthYear: 1975
      }
    };
  },
  methods: {
    handleDatachanged: function(personData) {
      this.person.name = personData.name;
      this.person.birthYear = personData.birthYear;
    }
  }
};
</script>
```
29
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
30
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
  data: function() {
    return {
      persondata: {
        name: null,
        birthYear: null
      }
    };
  },
  created: function() {
    this.persondata.name = this.personprop.name;
    this.persondata.birthYear = this.personprop.birthYear;
  },
  methods: {
    nav: function() {
      this.$emit("datachanged", this.persondata);
      this.$router.push("/sideb");
    }
  }
};
</script>
```
31
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
  created: function() {
    for (let t of this.trekningerProp) {
      this.trekninger.push(t);
    }
  },
  methods: {
    lagDatoTekstForVisning: function(dato) {
      return dato
        .toLocaleString()
        .replace(",", "")
        .substr(0, 15);
    },
    lagTekstListe: function(liste) {
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
32
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
  created: function() {
    for (let p of this.personerProp) {
      this.liste.push(p);
    }
  },
  methods: {
    velgAlleEllerIngen: function() {
      let verdi = !this.velgAlle;
      for (let person of this.liste) {
        person.erValgt = verdi;
      }
    },
    slettPerson: function(id) {
      let index = this.liste.findIndex(p => p.id === id);
      if (index == -1) return;
      this.liste.splice(index, 1);
      this.$emit("oppdatert-personliste", this.liste);
    },
    leggTilPerson: function() {
      const id =
        this.liste
          .map(p => p.id)
          .reduce((max, value) => Math.max(max, value), -1) + 1;
      this.liste.push({ id: id, navn: this.nyPerson, erValgt: true });
      this.nyPerson = "";
      this.$emit("oppdatert-personliste", this.liste);
    },
    trekk: function() {
      this.$emit("trekk", this.trekkAntall);
    }
  }
};
</script>
```
33
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
1
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
2
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
1
```js
async function testPost() {
    let files = {
        files: {
            "index.html": { "content": "<h1>Hallo</h1>", "isBinary": false },
            "index.js": { "content": "console.log('hello!')", "isBinary": false },
            "package.json": { "content": { "dependencies": {} } }
        }
    }

    let url = 'https://codesandbox.io/api/v1/sandboxes/define?json=1';
    let resultat = await axios.post(url, files);
    let sandboxId = resultat.data.sandbox_id;
}
```
## 19 - Kodegenerering og metadata
1
```
https://api.chucknorris.io/jokes/random
https://api.chucknorris.io/jokes/random?category={category}
https://api.chucknorris.io/jokes/categories
https://api.chucknorris.io/jokes/search?query={query}
```
2
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
3
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
4
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
5
```js
random = async () => await chuckNorrisRestKall('random', {} ); 
randomCategory = async (category) => await chuckNorrisRestKall('random', {category} ); 
categories = async () => await chuckNorrisRestKall('categories', {} ); 
searchQuery = async (query) => await chuckNorrisRestKall('search', {query} );
```
6
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
7
```js
let urler = [
    'https://api.chucknorris.io/jokes/random',
    'https://api.chucknorris.io/jokes/random?category={category}',
    'https://api.chucknorris.io/jokes/categories',
    'https://api.chucknorris.io/jokes/search?query={query}'
];
```
8
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
9
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
10
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
11
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
12
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
13
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
14
```html
<skjema-visning :person="{navn: 'Terje Kolderup', fødselsår: 1975}"></skjema-visning>
```		
15
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
16
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
17
```js
let komponenter = {
    overskrift: function (data) {},
    skjemaVisning: function (data, metadata, index) {},
    listeVisning: function (data, metadata) {},
    meny: function (data, metadata) {},
};
```
18
```js
overskrift: function (data) {
    let p = data.tekst ? `<p>${data.tekst}</p>` : '';
    return `<div class="sideElement" style="grid-area: overskrift">
                <h3>${data.overskrift}</h3>
                ${p}
            </div>`;
}
```
19
```js
meny: function (data, metadata) {
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
20
```js
sider: {
    "forside": {
        visningsnavn: 'Hjem',
    },
    "kategoriListe": {
        visningsnavn: 'Kategorier',
    },
    "produktListe": {
        visningsnavn: 'Alle produkter',
    },
    "enkeltProdukt": {
    },
    "kontaktOss": {
        visningsnavn: 'Kontakt oss',
    }
```
21
```js
skjemaVisning: function (data, metadata, index) {
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
22
```js
listeVisning: function (data, metadata) {
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
23
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
24
```js
[
    { navn: "Gullskje 22cm", pris: 990, kategori: "skje" },
    { navn: "Sølvskje 22cm", pris: 190, kategori: "skje" },
    { navn: "Stålskje 22cm", pris: 19, kategori: "skje" },
    { navn: "Gullkniv 22cm", pris: 990, kategori: "kniv" },
    { navn: "Sølvkniv 22cm", pris: 190, kategori: "kniv" },
    { navn: "Stålkniv 22cm", pris: 19, kategori: "kniv" },
    { navn: "Gullgaffel 22cm", pris: 990, kategori: "gaffel" },
    { navn: "Sølvgaffel 22cm", pris: 190, kategori: "gaffel" },
    { navn: "Stålgaffel 22cm", pris: 19, kategori: "gaffel" }
]
```
25
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
26
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
27
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
28
```js
sider: {
    "forside": {
        visningsnavn: 'Hjem',
        mal: "infoSide",
        data: { "overskrift": "tekster.forside", "skjemaVisning": "tekster.info" },
        metadata: { "skjemaVisning": "forside", "meny": "sider" },
    },
    "kategoriListe": {
        visningsnavn: 'Kategorier',
        mal: "listeSide",
        data: { "overskrift": "tekster.kategorier", "listeVisning": "kategorier" },
        metadata: { "meny": "sider", "listeVisning": "kategorier" },
    },
    "produktListe": {
        visningsnavn: 'Alle produkter',
        mal: "listeSide",
        data: { "overskrift": "tekster.produkter", "listeVisning": "produkter" },
        metadata: { "listeVisning": "produkt", "meny": "sider" }
    },
    "enkeltProdukt": {
        mal: "infoSide",
        data: { "overskrift": "tekster.produkt", "skjemaVisning": "produkter" },
        metadata: { "skjemaVisning": "produkt", "meny": "sider" }
    },
    "kontaktOss": {
        visningsnavn: 'Kontakt oss',
        mal: "infoSide",
        data: { "overskrift": "tekster.kontaktOss", "skjemaVisning": "tekster.kontaktOss.felt" },
        metadata: { "skjemaVisning": "kontaktOss", "meny": "sider" }
    }
}
```
29
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
30
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
