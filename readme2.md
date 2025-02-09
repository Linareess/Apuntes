# Bienvenidos a la página de Apuntes de *"Llenguatge de marques"*


ASIX1 - Curso 2425

---

## Índice

- [Aprendizaje Markdown](#aprendizaje-markdown)
- [GitHub](#github)
  - [Creación de repositorio](#creacion-de-repositorio)
  - [Comandos principales](#comandos-principales)
- [HTML](#html)
  - [Elementos básicos](#elementos-basicos)
  - [Formularios](#formularios)
  - [Tablas](#tablas)
  - [Posicionamiento](#posicionamiento)
- [CSS](#css)
  - [Fundamentos](#fundamentos)
  - [Diseño Responsive](#diseno-responsive)
- [Validación HTML](#validacion-html)
- [Recursos](#recursos)

---
# Markdown

## Sintaxis básica

```markdown
# Título principal
## Segundo nivel 
### Tercer nivel 
#### Cuarto nivel
##### Quinto nivel
###### sexto nivel de encabezado

*Texto en cursiva*  
**Texto en negrita**  
**_Texto combinado_**  
~~Texto tachado~~  

Estos son los apuntes de *0373* del ciclo formativo de _ASIX_ o **DAW** del curso __2425__

1. Primer titulo de lista
    1. Primer elemento de la lista 1
    2. Segundo elemento de la lista 1

2. Segundo titulo de la lista
    * Primer elemento de la lista 2
    * Segundo elemento de la lista 2
3. Tercer punto de la lista

- Primer punto de lista desordenada
* Segundo punto de lista desordenada
+ Tercer punto de lista desordenada

[Enlace](https://google.com "Título opcional")
![Imagen](img/Señorconcomputador.png "Descripción")
```
---

# GitHub

## Creación de repositorio

1. Click en **New** desde GitHub.
2. Personalizar:
   - **Nombre**: Identificador único
   - **Visibilidad**: Público/Privado
   - **README**: Incluir archivo inicial
3. Activar **GitHub Pages** para hosting.

## Comandos principales

```bash
git init                # Inicializar repositorio
git clone <url>         # Clonar repositorio remoto
git add .               # Preparar cambios
git commit -m "mensaje" # Confirmar cambios
git push origin main    # Subir a repositorio remoto
git pull                # Actualizar desde remoto
```

---

# HTML

## mostrar codigo
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Título página</title>
</head>
<body>
    <h1>Encabezado principal</h1>
    <p>Párrafo con <strong>énfasis</strong></p>
    <img src="logo.jpg" alt="Logo descriptivo">
</body>
</html>
```
La primer clase de **_markdown_** y HTML pueden anidarse en VS code

## Formularios

```html
<form action="/procesar" method="POST">
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" required>
    
    <fieldset>
        <legend>Preferencias</legend>
        <select name="curso">
            <option value="ASIX">ASIX</option>
            <option value="DAW">DAW</option>
        </select>
    </fieldset>
    
    <textarea placeholder="Comentarios..."></textarea>
    <button type="submit">Enviar</button>
</form>
```

## Tablas

```html
<table border="1">
    <thead>
        <tr>
            <th colspan="2">Datos</th>
        </tr>
    </thead>
    <tbody>
        <tr align="center">
            <td>ASIX1</td>
            <td>24-25</td>
        </tr>
    </tbody>
</table>
```

## Posicionamiento

```css
.container {
    position: relative;
    width: 300px;
    height: 200px;
    overflow: hidden;
}

.flotante {
    position: absolute;
    top: 20px;
    left: 50%;
}
```

---

# CSS

## Fundamentos

Tres métodos de aplicación:

### Inline:

```html
<p style="color: blue;">Texto azul</p>
```

### Interno:

```html
<style>
    body {
        background: #f0f0f0;
    }
</style>
```

### Externo:

```html
<link rel="stylesheet" href="estilos.css">
```

## Diseño Responsive

### Media Queries

```css
/* Mobile First */
body { background: lightblue; }

/* Tablet */
@media (min-width: 768px) {
    body { background: lightgreen; }
}

/* Escritorio */
@media (min-width: 1024px) {
    body { background: lavender; }
}
```

### Flexbox

```css
.contenedor {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}

.item {
    flex: 1 0 200px;
    margin: 10px;
}
```

---

# Validación HTML

1. Acceder al **Validador W3C**.
2. Seleccionar método de validación:
   - **Subir archivo**
   - **Introducir URL**
   - **Pegar código directamente**
3. Verificar el codigo
4. Corregir errores reportados.
5. Repetir la operacion hasta eliminar los errores.

---

# Recursos y ayudas

- [Guía completa HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [Documentación CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
- [GitHub Oficial](https://github.com/)

