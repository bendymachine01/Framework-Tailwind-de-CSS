# Taller Tailwind CSS

## Descripción

En este proyecto se desarrolla la guía práctica de Tailwind CSS utilizando HTML y el CDN de Tailwind.

Tailwind CSS permite diseñar páginas web utilizando clases de utilidad directamente en el HTML. Estas clases permiten controlar colores, texto, espaciado, bordes, sombras, distribución y efectos interactivos.

## Herramientas

- Visual Studio Code
- Navegador web
- HTML5
- Tailwind CSS mediante CDN

## Configuración

Para utilizar Tailwind se agregó el CDN dentro del `<head>`:

```html
<script src="https://cdn.tailwindcss.com"></script>
```

## Ejemplo básico

```html
<h1 class="text-2xl font-bold text-sky-600">
    ¡Hola Mundo con Tailwind!
</h1>
```

En este ejemplo:

- `text-2xl`: cambia el tamaño del texto.
- `font-bold`: coloca el texto en negrita.
- `text-sky-600`: cambia el color del texto.

## Reto 1: Modo Neón / Modo Oscuro

Se cambió el fondo del `body` a `bg-slate-950`, la tarjeta a `bg-slate-900`, los textos a colores claros y el botón a `bg-emerald-500` con `hover:bg-emerald-600`.

Ejemplo:

```html
<body class="bg-slate-950 min-h-screen p-6">

<button class="bg-emerald-500 hover:bg-emerald-600 text-white rounded-xl">
    Seguir Perfil
</button>
```

## Reto 2: Barra de Estadísticas

Se agregó una barra con tres estadísticas:

- Proyectos: 14
- Seguidores: 1.2k
- Nivel: 85

Código utilizado:

```html
<div class="flex justify-around bg-slate-800 rounded-xl p-3 mb-4">
    <div>
        <p class="font-bold text-white">14</p>
        <p class="text-xs text-slate-400">Proyectos</p>
    </div>

    <div>
        <p class="font-bold text-white">1.2k</p>
        <p class="text-xs text-slate-400">Seguidores</p>
    </div>

    <div>
        <p class="font-bold text-white">85</p>
        <p class="text-xs text-slate-400">Nivel</p>
    </div>
</div>
```

## Reto 3: Grilla Responsive

Se creó una grilla con tres tarjetas. En pantallas pequeñas se muestra una columna y desde el tamaño `md` se muestran tres columnas.

```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-5xl">
```

Clases principales:

- `grid`: activa la grilla.
- `grid-cols-1`: una columna.
- `md:grid-cols-3`: tres columnas en pantallas medianas.
- `gap-6`: agrega espacio entre las tarjetas.
- `max-w-5xl`: limita el ancho del contenido.

## Efectos interactivos

También se utilizaron clases `hover:` y `transition` para crear efectos al pasar el mouse sobre las tarjetas y botones.

Ejemplo:

```html
<button class="bg-emerald-500 hover:bg-emerald-600 transition">
    Seguir Perfil
</button>
```

## Resultado

El proyecto final contiene:

1. Un diseño en modo oscuro/neón.
2. Una barra de estadísticas.
3. Tres tarjetas organizadas en una grilla responsive.
4. Efectos `hover` y transiciones.
5. Diseño adaptable a diferentes tamaños de pantalla.

## Estructura del proyecto

```text
tailwind_css/
├── index.html
└── README.md
```
