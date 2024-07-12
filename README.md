# GSAP Vanilla Responsive Menu

## Description

Este proyecto es una aplicación web en HTML5, CSS3, VanillaJS y Vite, que implementa un menú responsive y animaciones utilizando GSAP. El menú incluye elementos animados que se expanden y colapsan al hacer clic o hover.

[![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)]()
[![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)]()
[![Vite](https://img.shields.io/badge/Vite-B73BFE?style=for-the-badge&logo=vite&logoColor=FFD62E)]()

![Code](public/assets/doc1.webp)

## Funcion personalizada para dividir texto

```javascript
function splitTextIntoSpans(selector) {
  let elements = document.querySelectorAll(selector);
  elements.forEach((element) => {
    let text = element.innerText;
    let splitText = text
      .split("")
      .map((char) => `<span>${char === " " ? "&nbsp;&nbsp;" : char}</span>`)
      .join("");
    element.innerHTML = splitText;
  });
}

splitTextIntoSpans(".menu-link p");
```

## Instalación

1. Clona este repositorio:
   ```sh
   git clone https://github.com/tuusuario/gsap-vanilla-responsive-menu.git
   ```
2. Navega al directorio del proyecto:
   ```sh
   cd gsap-vanilla-responsive-menu
   ```
3. Instala las dependencias:
   ```sh
   npm install
   ```

## Uso

1. Inicia el servidor de desarrollo:
   ```sh
   npm run dev
   ```
2. Abre tu navegador y visita `http://localhost:3000`.
