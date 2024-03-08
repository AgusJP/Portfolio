---
layout: ../../layouts/BlogLayout.astro
title: Patrones de Diseño - Patrón Singleton 🎯
author: Agustín Jiménez Polonio
description: Como garantizar que una clase solo tenga una instancia y proporcionar un punto de acceso global a ella.
image:
  url: "/assets/posts/singleton-pattern.webp"
  alt: "Patrón singleton thumbnail"
pubDate: Feb 27, 2024
tags: ["patrones de diseño", "backend"]
---

# Patrones de Diseño - Patrón Singleton 🎯

El patrón Singleton es un patrón de diseño creacional que asegura que una clase solo tenga una instancia, y que proporciona un punto de acceso global a dicha instancia.

<br>

## ¿Cómo funciona?

El patrón Singleton define una clase con un constructor privado y un método estático para obtener la instancia única. La primera vez que se llama al método ```getInstance()```, se crea la instancia y se guarda en una variable privada. Las llamadas posteriores al método `getInstance()` devolverán la misma instancia.

<br>

<div class="video-container">
  <iframe src="https://www.youtube.com/embed/ekeb470kkAo" title="Patrones de Diseño: Patrón Singletone ♻" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

<br>

## Beneficios:

- **Control sobre la creación de objetos:** Se asegura que solo haya una instancia de la clase.
- **Acceso global a la instancia:** Se puede acceder a la instancia desde cualquier lugar del código.
- **Facilidad de uso:** El patrón Singleton simplifica el acceso a objetos singulares.

<br>

## Utilidad:

El patrón Singleton es útil para:

- Implementar objetos singulares como gestores de configuración, caches o pools de conexiones.
- Controlar el acceso a recursos compartidos.
- Garantizar que solo haya una instancia de un objeto en memoria.

<br>

## Recursos adicionales:

- Wikipedia: [Patrón Singleton](https://en.wikipedia.org/wiki/Singleton_pattern)
- Refactoring Guru: [Patrón Singleton](https://refactoring.guru/design-patterns/singleton)

<br>

El patrón Singleton puede ser un poco controvertido, ya que puede ser visto como una violación del principio de encapsulación. Sin embargo, el patrón Singleton puede ser útil en algunos casos específicos.

<style>
  .video-container {
    position: relative;
    width: 95%;
    padding-bottom: 56.25%; 
    overflow: hidden;
    margin-top: 2.5em;
    margin-bottom: 2.5em;
  }
    
  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

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

  p {
    max-width: 70ch; 
    color: #cbd1d4;
  }

  p, li {
    color: #cbd1d4;
  }

  @media screen and (max-width: 770px) {
    .video-container {
      width: 100%;
    }
    h1 {
      font-size: 2em;
    }
  }
</style>
