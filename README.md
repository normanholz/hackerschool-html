# hackerschool-html
Repository for the Hackerschool HTML Course

# HTML Dokumentation:
- https://www.w3schools.com/tags/
- https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes

# CSS Dokumentation:
  
- https://www.mediaevent.de/css/
- https://wiki.selfhtml.org/wiki/Box-Modell
- https://developer.mozilla.org/de/Learn/Getting_started_with_the_web/CSS_basics
- https://blog.kulturbanause.de/2013/07/einfuhrung-in-das-flexbox-modell-von-css/
- https://wiki.selfhtml.org/wiki/Schnell-Index/CSS
- https://www.w3schools.com/css/css3_animations.asp
- https://www.w3schools.com/cssref/

# Farben

- https://htmlcolorcodes.com/color-names/

# Kursnotizen

## Schritt 1:

`<h1>Hallo Hacker School.</h1>`

## Schritt 2: Einfache Textformatierung

`Ich bin unformatierter Text.`

`<b>Hallo ich bin fett.</b>`

`<strong>Ich bin auch dick.</strong>`

`<i>Ich bin schief.</i>`

`<em>Ich auch.</em>`

## Schritt 3: Schachtelung von Elementen

`<strong>Ich bin immmer dick und manchmal <em>schief</em> und <del>durchgestrichen</del>.</strong>`

## Schritt 4: Bilder

`mkdir images`

`cd images`

`curl "https://www.hacker-school.de/fileadmin/env/default/images/logo.png"`

`<img alt="Ich bin ein Bild" src="images/meme.jpg" />`

## Schritt 5: Eigenschaften der Elemente

`<h1 style=„color: orange“>Hallo Hacker School.</h1>`

## Schritt 6: Seitenelemente Head und Body

- Chrome Dev Tools

`<html></hmtl`

`<head></head>`

`<body></body>`

`<title>Hacker School</title>`

## Schritt 7: Elemente Paragraph und Listen

`<p></p>`

`<ol></ol>`

`<ul></ul>`

`<li></li>`

## Schritt 8: Verlinkung zu anderen Seiten

`mkdir pages`

`<a href=""></a>`

## Schritt 9: Divs als neutrale Elemente mit Eigenschaften

`<div style="color: orange">`

## Schritt 10: Bildgröße per CSS steuern

`<img style="width: 100%; height: auto" alt="Ich bin ein Bild" src="../images/meme.jpg"/>`

## Schritt 11: DRY CSS Stylesheet im Head Element

    <style>
         img {
             width: 100%;
             height: auto;
         }
     </style>`
     
    <style>
         p {
             color: cornflowerblue;
         }
         #htmlElemente {
             color: orange;
         }
     </style>   
     
    <div id="htmlElemente">
    
## Schritt 12: CSS Box Model

<img src="https://wiki.selfhtml.org/images/thumb/f/f3/Box-Modell.svg/600px-Box-Modell.svg.png"/>


    <head>
        <title>CSS Box Model</title>
    </head>
    <style>
        h1 {
            border: 1px solid black;
            text-align: center;
            padding: 20px;
            margin: 20px;
        }
    </style>
    <body>
    
    <h1>Das CSS Box Model</h1>
    
    <img alt="CSS Box Model" src="https://wiki.selfhtml.org/images/thumb/f/f3/Box-Modell.svg/600px-Box-Modell.svg.png"/>
    
    </body>
    </html>    
         
 ## Schritt 13: Schriften anpassen
 
     body {
         font-family: Arial, sans-serif;
     }
    
     h1 {
         text-align: center;
         text-transform: uppercase;
         padding: 20px;
         color: #0000FF;
     }
    
     h2 {
         text-align: center;
         margin-bottom: 50px;
         text-transform: uppercase;
         font-weight: 300;
     }
     
 ## Schritt 14: Layouts mit Flexbox
 
     <head>
         <title>Coole Bilder</title>
         <style>
             .flex-container {
                 border: solid 1px black;
                 width: 100%;
                 height: auto;
                 display: flex;
                 justify-content: center;
                 align-items: center;
     
             }
     
             img {
                 width: 300px;
                 padding: 20px;
             }
     
             h1 {
                 border: 1px solid black;
                 text-align: center;
                 padding: 20px;
                 margin: 20px;
             }
         </style>
     </head>
     <body>
     
     <h1>Coole Bilder</h1>
     
     <div class="flex-container">
         <div class="flex-item">
             <img alt="" src="../images/meme.jpg"/>
         </div>
         <div class="flex-item">
             <img alt="" src="../images/meme.jpg"/>
         </div>
         <div class="flex-item">
             <img alt="" src="../images/meme.jpg"/>
         </div>
     </div>
     
     </body>
     </html>
     
     
## Schrit 15: Animationen mit CSS

    <head>
        <title>Coole Animationen</title>
        <style>
            .flex-container {
                width: 100%;
                display: flex;
                justify-content: center;
                align-items: center;
            }
    
            h1 {
                border: 1px solid black;
                text-align: center;
                padding: 20px;
                margin: 20px;
            }
    
            div {
                width: 100px;
                height: 100px;
                padding: 20px;
            }
    
            div#animated-box-1 {
                background-color: red;
                animation-name: animation-box-1;
                animation-duration: 4s;
                animation-iteration-count: infinite;
            }
    
            div#animated-box-2 {
                position: relative;
                background-color: red;
                animation-name: animation-box-2;
                animation-duration: 4s;
                animation-iteration-count: infinite;
            }
    
            div#animated-box-3 {
                background-color: green;
                animation-name: animation-box-3;
                animation-duration: 4s;
                animation-iteration-count: infinite;
            }
    
            @keyframes animation-box-1 {
                from {background-color: red;}
                to {background-color: yellow;}
            }
    
            @keyframes animation-box-2 {
                0%   {background-color:red; left:0px; top:0px;}
                25%  {background-color:yellow; left:200px; top:0px;}
                50%  {background-color:blue; left:200px; top:200px;}
                75%  {background-color:green; left:0px; top:200px;}
                100% {background-color:red; left:0px; top:0px;}
            }
    
            @keyframes animation-box-3
            {
                0% {transform: rotate(0deg);left:0px;}
                25% {transform: rotate(20deg);left:0px;}
                50% {transform: rotate(0deg);left:500px;}
                55% {transform: rotate(0deg);left:500px;}
                70% {transform: rotate(0deg);left:500px;background:#1ec7e6;}
                100% {transform: rotate(-360deg);left:0px;}
            }
    
        </style>
    </head>
    <body>
    
    <h1>Coole Animationen</h1>
    
    <div class="flex-container">
        <div class="flex-item">
            <div id="animated-box-1"></div>
        </div>
        <div class="flex-item">
            <div id="animated-box-2"></div>
        </div>
        <div class="flex-item">
            <div id="animated-box-3"></div>
        </div>
    </div>
    
    </body>
    </html>
