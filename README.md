# hackerschool-html
Repository for the Hackerschool HTML Course 

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
     
