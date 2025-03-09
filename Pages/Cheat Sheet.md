# Cheat Sheet

## Nagłówki

 

```# Nagłówek 1 stopnia```  
```# Nagłówek 2 stopnia```  
```# Nagłówek 3 stopnia```

 

## Formatowanie tekstu

 

```*Pochyły*``` *Pochyły*  
```__Pogrubiony__``` __Pogrubiony__  
```__*Pochyły i pogrubiony*__``` __*Pochyły i pogrubiony*__  
Dodając na koniec lini co najmniej dwie spacje spowodujesz przejście do nowej lini nie kończąc akapitu.

 

## Fragmenty kodu

 

````markdown
```język programowania np.: javascript
Fragment kodu np.: let zmienna = 7;
```
````
```javascript
Fragment kodu np.: let zmienna = 7;
```

 

## Zapis matematyczny

 
|Formuła|Render|
|:-----:|:----:|
|``` $$ 2^2=4 $$ ```| $$2^2=4$$  |
|``` $$ 10\times2=5 $$ ```| $$10\times2=5$$  |
|``` $$ 10x \times2=20x $$ ```| $$10x \times2=20x$$  |
|``` $$ 2\phantom{0}048 $$ ```| $$ 2\phantom{0}048 $$  |
|``` $$ \\% $$ ```|  $$ \\% $$  |
|``` $$ \And\And $$ ```| $$\And\And$$  |

[Pozostałe formuły renderowana z biblioteki KaTeX.js](https://katex.org/docs/support_table)
 

## Obraz

 

```![Tekst alternatywny opisujący obraz, który jest wyświetlany, gdy obraz nie może zostać załadowany.](lokalizacja pliku obrazka)```  
np.:  
```markdown
![Zimowa góra.](/basic-preset-image.jpg)
```

![Tekst alternatywny opisujący obraz, który jest wyświetlany, gdy obraz nie może zostać załadowany.](basic-preset-image.jpg)

```markdown
![tekst alternatywny](/Images/plik.png)
```
 

## Listy automatyczne

 

Aby wykonać zagnieżdżenie listy użyj tabulacji.

### Lista numerowana

Zwróć uwagę, że dane podpunkty będą kontynuacją pierwszej podanej liczby dla danego zagnieżdżenia, a potem nie ma znaczenia, jaką liczbę podasz, aczkolwiek warto pisać składnie i logicznie:

1. Pierwszy
    14. drugi
    3. trzeci
9. czwarty
    1. piąty
        2. szósty

```markdown
1. Pierwszy
    14. drugi
    3. trzeci
9. czwarty
    1. piąty
        102. szósty
```

### Lista nienumerowana

Możesz wykorzystać znak plusa, minusa lub gwiazdki:

- pierwszy
    + drugi
        - trzeci
+ czwarty
    * piąty
        * szósty

```markdown
- pierwszy
    + drugi
        - trzeci
+ czwarty
    * piąty
        * szósty
```

 

# Znaczniki HTML i specjalne generowane w JavaScript

 

## Element szczegółu

 

<details>
<summary>Kategorie produktów spożywczych</summary>

* Warzywa
* Owoce
* Mieso
* Nabiał

</details>

```markdown
<details>
<summary>Kategorie produktów spożywczych</summary>

* Warzywa
* Owoce
* Mieso
* Nabiał

</details>
```
 

## Karty

 

<div data-tabs>
    <div class="tabs">
        <b>Tab 1</b>
        <b>Tab 2</b>
    </div>
    <div class="active">
        <h3>Tab 1</h3>
        <p>Zawartość pierwszej karty.</p>
    </div>
    <div>
        <h3>Tab 2</h3>
        <p>Zawartość drugiej karty.</p>
    </div>
</div>

```html
<div data-tabs>
    <div class="tabs">
        <b>Tab 1</b>
        <b>Tab 2</b>
    </div>
    <div class="active">
        <h3>Tab 1</h3>
        <p>Zawartość pierwszej karty.</p>
    </div>
    <div>
        <h3>Tab 2</h3>
        <p>Zawartość drugiej karty.</p>
    </div>
</div>
```

 

## Hinty

 

<div data-hint="info">

To jest hint __informacyjny__.

</div>

```html
<div data-hint="info">

To jest hint __informacyjny__.

</div>
```

<div data-hint="success">

To jest hint __sukcesu__.

</div>

```html
<div data-hint="success">

To jest hint __sukcesu__.

</div>
```

<div data-hint="warning">

To jest hint __ostrzegawczy__.

</div>

```html
<div data-hint="warning">

To jest hint __ostrzegawczy__

</div>
```

<div data-hint="danger">

To jest hint __niebezpieczeństwa__.

</div>

```html
<div data-hint="danger">

To jest hint __niebezpieczeństwa__.

</div>
```

 

## Embed z YouTube

 

<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=Eir45MTGwuEeP6D7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

  -->