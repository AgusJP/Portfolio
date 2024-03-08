---
layout: ../../layouts/BlogLayout.astro
title: Patrones de Diseño - Patrón Builder 🏗️
author: Agustín Jiménez Polonio
description: Un patrón de diseño creacional que separa la construcción de un objeto complejo de su representación. 
image:
  url: "/assets/posts/builder-pattern.webp"
  alt: "Patrón builder thumbnail"
pubDate: Feb 26, 2024
tags: ["patrones de diseño", "backend"]
---

# Patrones de Diseño - Patrón Builder 🏗️

El Patrón Builder es un patrón de diseño creacional que se utiliza para construir objetos complejos paso a paso. Su principal objetivo es separar la construcción de un objeto de su representación, permitiendo que el mismo proceso de construcción pueda crear diferentes tipos y representaciones del objeto.

<br>

<div class="video-container">
  <iframe src="https://www.youtube.com/embed/LnNmC4p9m_o" title="Patrones de Diseño: Patrón Builder 🏗️" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

<br>

Este patrón es útil cuando la construcción de un objeto requiere un proceso complejo o cuando se necesitan diferentes representaciones del mismo objeto. También promueve un código más limpio y mantenible al encapsular el proceso de construcción dentro de clases separadas, lo que facilita la extensión y la modificación en el futuro.

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
