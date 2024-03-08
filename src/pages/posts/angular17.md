---
layout: ../../layouts/BlogLayout.astro
title: Todas las novedades de Angular 17 ✨
author: Agustín Jiménez Polonio
description: Experimenta un desarrollo web más intuitivo y eficiente con SSR mejorado, sintaxis de control de flujo renovada, carga diferida de componentes y mucho más.
image:
  url: "/assets/posts/angular17.webp"
  alt: "Angular 17 thumbnail"
pubDate: Feb 11, 2024
tags: ["angular", "frontend"]
---

# ¡Angular 17: Un Renacimiento Impresionante!

## Introducción

¡Estoy emocionado por compartir las increíbles novedades de Angular 17! Desde la versión 16 con la llegada de los Standalone components y Signals, Angular no ha parado de sorprenderme. El renacimiento e introducción a Angular con la versión 17 es impresionante.

## Novedades

### ⚡ Flujo de Control Mejorado:
Angular 17 introduce una nueva sintaxis para estructuras de control como @Switch, @If, y @For. Esta sintaxis busca mejorar la experiencia de desarrollo, haciendo que el código sea más ergonómico y simplificado para nuevos desarrolladores.

```javascript
  //@if
  @if (showHello) {
    <h2>Hello</h2>
  } 
  @else if (showGoodbye) {
    <h2>Goodbye</h2>
  } 
  @else {
    <h2>See you later</h2>
  }

  //@for
  @for (item of items; track item.id) {
    {{ item.name }}
  }

  //@switch
  @switch (color) {
    @case ("red") {
      <div>Red</div>
    }
    @case ("blue") {
      <div>Blue</div>
    }
  }
```

<br>

### 🔄 Carga Diferida a Nivel de Componente ( @Defer Deferrable views): 
Mi característica favorita. Evolución del lazy loading que permite hacer prefetch automático de componentes.

La sintaxis para utilizar esta función es sencilla y declarativa. Ofrece un control avanzado, gestionando errores, mostrando placeholders, y activando acciones según distintos triggers, como tiempo de carga o interacciones.

Al cargar selectivamente componentes, esta característica tiene el potencial de mejorar significativamente el rendimiento de la página web.

```javascript
<div #greeting>Hello!</div>

@defer (on hover(greeting)) {
  <calendar-cmp />
} @placeholder {
  <div>Calendar placeholder</div>
}
```

<br>

### 🚀 Mejoras en el Entorno de Desarrollo (Vite + esbuild):
Se introduce el uso de Vite como entorno de desarrollo, brindando un manejo más eficiente del “Hot Reloading” y una recarga instantánea, mejorando significativamente la experiencia del desarrollador. Además con el uso de esbuild como enpaquetador se mejora significativamente la velocidad de construcción de la aplicación.

<br>

### 🖥️ Server Side Rendering (SSR) Mejorado:
Angular ahora integra el SSR como parte fundamental del framework, ofreciendo un equilibrio óptimo entre rendimiento y funcionalidad. ¡Una excelente noticia para aquellos que buscan mejorar el SEO y la velocidad de carga!

Para crear una nueva aplicación con SSR:
```
ng new --ssr
```

Para agregar SSR a un proyecto existente, use el comando Angular ``CLI ng`` add:
```
ng add @angular/ssr

```
<br>

### 🌐 Retrocompatibilidad Garantizada:
Angular 17 sigue siendo fiel a sus raíces, permitiendo la retrocompatibilidad con módulos y sintaxis antiguas. Esto facilita la transición para proyectos existentes y muestra el compromiso con la estabilidad.

```
ng update @angular/core@17
```

<br>

## Recursos adicionales

- Nueva página web de Angular: https://angular.dev/
- Blog oficial de Angular: https://blog.angular.io/

<br>

Estos son solo algunos ejemplos para ilustrar las nuevas características. Te recomiendo explorar la documentación oficial de Angular para obtener más información y ejemplos en profundidad.


<style>
  h1 {
    width: 100%;
    margin-top: 0;
    color: #2cc9ff;
    font-size: 3em;
  } 

  a {
    color: #cbd1d4;
    font-weight: bold
  }

  main {
    width: 100%;
    font-size: 20px;
    padding: 0 10px 0 10px;
  }
  
  pre {
    width: 100%;
    padding: 20px;
    border-radius: 8px;
    font-size: .8em;
  }

  code {
    width: 100%;
  }

  p {
    max-width: 70ch; 
    color: #cbd1d4;
  }

  @media screen and (max-width: 770px) {
    h1 {
      font-size: 2em;
    }
  }
</style>