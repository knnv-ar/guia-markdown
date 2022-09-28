# Guía rápida de Markdown

Realizada por Raúl Federico Lacabanne (aka: knnv-ar) en estrecha relación a los documentos de la referencia. Fecha: 2022/06/30

## Encabezados

Markdown dispone de seis tañamos de encabezados:

# Encabezado 1 (h1)

## Encabezado 1 (h2)

### Encabezado 3 (h3)

#### Encabezado 4 (h4)

##### Encabezado 5 (h5)

###### Encabezado 6 (h6)

---

## Texto de párrafo

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec finibus et nulla eget euismod. Suspendisse vitae rutrum ex, sed ultricies odio. Sed magna est, convallis non sem sed, blandit pulvinar felis. Aenean maximus lacus non nisi pellentesque cursus. Quisque vel aliquam elit. Proin in aliquet libero. Proin ipsum neque, molestie nec interdum ac, consectetur id velit. Nam accumsan varius accumsan. Suspendisse rutrum, leo posuere venenatis condimentum, sapien ligula tempus urna, nec sodales enim eros ut urna. Maecenas ut mattis eros, ac vehicula neque. Nulla ut justo velit. Quisque dictum, magna eget vestibulum dapibus, libero ipsum tincidunt purus, in egestas erat justo sit amet diam. Ut lacus erat, sollicitudin quis malesuada id, lacinia eget nibh.

---

## Estilos de texto

_\cursiva_\: _Este texto está en cursiva._

**Este texto está en negrita.**

~~Este texto está tachado.~~

**Este texto es _extremadamente_ importante**

**_Todo este texto es importante_**

La última palabra está escrita como <sup>superíndice</sup>.

La última palabra está escrita como <sub>subíndice</sub>.

---

## Listas

**Lista sin ordenar:**

- Item 1
- Item 2
  - Item 2a
  - Item 2b

**Lista ordenada:**

1. Item 1
2. Item 2
3. Item 3
   - Item 3a
   - Item 3b

**Lista de tareas**

* [x] Escribir anteproyecto (realizado)
* [ ] Corregir anteproyecto (pendiente)

---

## Enlaces

**Enlaces automáticos:**

http://github.com - enlace automático

**Enlaces con texto de referencia:**

[GitHub](http://github.com) - enlace con texto

---

## Cita de texto

Según las normas APA si el texto a citar tiene menos de 40 palabras "se debe poner así, entre comillas dobles".

Pero si el texto a citar tiene 40 o más palabras debe ser citado de la siguiente manera:

> Esta va a ser una cita muy larga, es decir, va a tener 40 o más palabras y la verdad es que no tengo otra cosa más que decir porque ya he dicho todo lo que tenía que expresar. Adios. (Lacabanne, 2022, pp 50-51)

---

## Códigos

**Código o comandos en la linea de texto:**

Para inicializar git en un directorio, dirigirse al mismo y desde allí tipear: `git init`.

**Bloque de código:**

Para crear un nuevo repositorio desde la línea de comando:

```bash
# Ejemplo de comandos en Bash
echo "# test" >> README.md
git init
git add README.md
git commit -m "Mi primer commit"
git branch -M main
git remote add origin https://github.com/knnv-ar/prueba.git
git push -u origin main
```

Observen que el ejemplo anterior se colorea distinto que el siguiente porque Markdown sigue un patrón de distribución de color en relación al lenguaje que se haya determinado al principio del bloque: el primero corresponde a Bash y el segundo a JavaScript:

```js
// Ejemplo en script en Javascript
function test() {
  console.log("look ma`, no spaces");
}
```

**Diferencias de código**

```diff
- This line is removed.
+ This line is added.
```

## Contenido colapsable
   
<details>
  <summary>Click acá</summary>
  
  ### Título
  1. Foo
  2. Bar
     * Baz
     * Qux

  ### El código

  ```js
  function logSomething(something) {
    console.log('Something', something);
  }
  ```
</details>

---

## Imágenes

**Se recomienda guardar las imágenes en una carpeta específica como por ejemplo `images`:**

![GitHub Logo](/images/GitHub_Logo.png)

![GitHub White Logo](/images/GitHub_Logo_White.png)

![Google Logo](/images/google-logo-6.png)

Formato: `![texto alternativo](url)`


## Referencias:

https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf

## Recursos

[Tutorial interactivo en castellano](https://www.markdowntutorial.com/es/)

---
https://github.com/zairahira/Markdown-cheatsheet/edit/main/README.md

# heading 1
## heading 2
### heading 3
### heading 4
#### heading 5

<!-- Italics -->
*this text is italics*

_italic_

<!-- Bold -->
**bold**

<!-- Strike Through-->
~~strike~~

<!-- Horizontal Line -->

--- 
___

## Block quotes

<!-- Block quote -->
> this is a block

## Links
<!--  links -->
[This is a link](inserlink.com)

[This is a link with tooltip](inserlink.com "tooltip")

## Lists

<!-- Unordered List -->
* item1
    * item2

<!--Ordered List-->

1. first item
2. second item

## Inline code block
<!-- inline code block-->
`<p></p>`

## Images
<!--Images-->

![Hollow Knight](hollo.jpg)


<!-- github md-->

## Code Blocks
### Bash code block

<!-- Bash script block -->

```bash
    npm install
    
```
### JS code block

<!-- JS Block-->

```javascript
function add(num1, num2){

}

```
### Python code block

<!-- Python block-->

```python
print("Hi there")
```

## Task list
<!-- task list -->
* [x] done
* [ ] not done

## Tables
<!-- tables -->
<!-- Note that :---: means center aligned -->
<!-- Note that ---: means right aligned -->
<!-- Note that :--- means left aligned -->

| Column 1 | Column 2 | Column 3 |
| :---: | :--- | ---: |
| Row 1, Column 1 | Row 1, Column 2 | Row 1, Column 3 |
| Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |
| Row 3, Column 1 | Row 3, Column 2 | Row 3, Column 3 |

## Diff
<!-- Diff -->
```diff
- This line is removed.
+ This line is added.
```

## Collapsible content
   <details>
          <summary>Click to see more!</summary>
          
            ## More awesoms tips!

            - item 1 
            - item 2
        </details>
