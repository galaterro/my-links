# My Links - Página de Enlaces Personales

Una página web sencilla estilo Linktree para mostrar enlaces a tus redes sociales, eventos y más.

## Características

- Diseño simple y elegante con Tailwind CSS
- Fácil de personalizar a través de un archivo JSON
- Iconos SVG incluidos para las redes sociales más populares
- Totalmente responsive

## Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/galaterro/my-links.git
   cd my-links
   ```

2. Instala las dependencias:
   ```bash
   npm install
   ```

3. Construye los estilos CSS:
   ```bash
   npx tailwindcss -i input.css -o output.css
   ```

4. Abre `index.html` en tu navegador o sube los archivos a tu servidor web.

## Cómo editar tus enlaces

Simplemente modifica el archivo `links.json` con tus propios datos:

1. En la sección `profile`, cambia:
   - `name`: Tu nombre o título
   - `description`: Una breve descripción
   - `image`: URL de tu foto de perfil 

2. En la sección `links`, cada enlace tiene:
   - `title`: Texto del botón
   - `url`: Enlace al que dirigirá
   - `icon`: (Opcional) Código SVG del icono

## Personalización

### Cambiar colores y estilos

Puedes personalizar la apariencia modificando directamente el archivo `index.html`. El proyecto utiliza Tailwind CSS, lo que facilita cambiar colores, espaciados y demás propiedades visuales.

Algunos ejemplos de personalización:

- Cambiar el fondo del gradiente: modifica las clases `from-gray-100 to-gray-200` en el elemento body
- Cambiar el color de los botones: modifica las clases `bg-gray-800 hover:bg-gray-700` en los enlaces
- Ajustar tamaños y espaciados: modifica los valores de padding (`p-*`), margin (`m-*`) y width (`w-*`)

### Añadir nuevos iconos

Puedes encontrar iconos SVG en sitios como:
- [Bootstrap Icons](https://icons.getbootstrap.com/)
- [Feather Icons](https://feathericons.com/)
- [Heroicons](https://heroicons.com/)

Copia el código SVG del icono y úsalo en el campo `icon` de tu enlace en `links.json`.

## Estructura del proyecto

```
my-links/
├── index.html         # Página principal
├── links.json         # Configuración de perfil y enlaces
├── input.css          # Archivo de entrada para Tailwind CSS
├── output.css         # Archivo CSS compilado (generado)
├── assets/            # Carpeta para imágenes y otros recursos
│   └── image.webp     # Imagen de perfil por defecto
└── package.json       # Configuración de dependencias
```

## Despliegue

### GitHub Pages

1. Sube tu repositorio a GitHub
2. Activa GitHub Pages en la configuración del repositorio
3. Selecciona la rama principal como fuente

### Netlify/Vercel

También puedes desplegar fácilmente en servicios como Netlify o Vercel importando tu repositorio de GitHub.

## Contribuir

Si quieres contribuir a este proyecto:

1. Haz un fork del repositorio
2. Crea una rama para tu función (`git checkout -b feature/nueva-funcion`)
3. Haz commit de tus cambios (`git commit -m 'Añadir nueva función'`)
4. Haz push a la rama (`git push origin feature/nueva-funcion`)
5. Abre un Pull Request

## Licencia

Este proyecto está licenciado bajo la licencia ISC - ver el archivo LICENSE para más detalles.