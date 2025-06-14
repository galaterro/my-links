# My Links - Página de Enlaces Personales

Una página web moderna estilo Linktree para mostrar enlaces organizados por categorías, con sistema de temas personalizable y diseño completamente responsive.

## 🌟 Características

- **🎨 Temas Personalizables**: Configura colores dinámicamente desde JSON
- **📱 Diseño Responsive**: Optimizado para móviles, tablets y desktop
- **🏷️ Categorización**: Organiza tus enlaces por categorías temáticas
- **⚡ Carga Rápida**: Sin frameworks pesados, JavaScript vanilla
- **🎯 Fácil Configuración**: Modifica todo desde un archivo JSON
- **🔗 Iconos SVG**: Incluye iconos para las principales redes sociales
- **🌐 Accesible**: Cumple con estándares de accesibilidad web
- **📦 Tecnologías Modernas**: Tailwind CSS v4, Google Fonts

## 🚀 Instalación Rápida

1. **Clona el repositorio**:
   ```bash
   git clone https://github.com/galaterro/my-links.git
   cd my-links
   ```

2. **Instala dependencias**:
   ```bash
   npm install
   ```

3. **Genera los estilos**:
   ```bash
   npx tailwindcss -i input.css -o output.css --watch
   ```

4. **¡Listo!** Abre `index.html` en tu navegador

## ⚙️ Configuración Personalizada

### 👤 Perfil Personal

Edita la sección `profile` en `links.json`:

```json
{
  "profile": {
    "name": "@TuUsuario",
    "description": "Tu descripción aquí",
    "image": "./assets/tu-imagen.webp"
  }
}
```

### 🎨 Personalización de Colores

Configura tu tema en la sección `theme`:

```json
{
  "theme": {
    "primaryColor": "#1f2937",    // Color principal
    "accentColor": "#3b82f6",     // Color de acento
    "textColor": "#ffffff"        // Color del texto
  }
}
```

### 🔗 Estructura de Enlaces

Organiza tus enlaces por categorías:

```json
{
  "categories": [
    {
      "title": "Redes Sociales",
      "links": [
        {
          "title": "Instagram",
          "url": "https://instagram.com/usuario",
          "icon": "<svg>...código SVG...</svg>"
        }
      ]
    }
  ]
}
```

## 🛠️ Scripts de Desarrollo

Añade estos scripts útiles a tu `package.json`:

```json
{
  "scripts": {
    "build": "npx tailwindcss -i input.css -o output.css",
    "dev": "npx tailwindcss -i input.css -o output.css --watch",
    "serve": "python -m http.server 8000"
  }
}
```

- `npm run build`: Compila CSS para producción
- `npm run dev`: Modo desarrollo con auto-recarga
- `npm run serve`: Servidor local de desarrollo

## 🎨 Recursos de Iconos

Encuentra iconos SVG gratuitos en:

- **[Bootstrap Icons](https://icons.getbootstrap.com/)** - Amplia colección de iconos
- **[Feather Icons](https://feathericons.com/)** - Iconos minimalistas
- **[Heroicons](https://heroicons.com/)** - Por los creadores de Tailwind
- **[Lucide](https://lucide.dev/)** - Fork moderno de Feather Icons

**💡 Tip**: Copia el código SVG y pégalo en el campo `icon` de tu enlace.

## 📁 Estructura del Proyecto

```
my-links/
├── 📄 index.html          # Página principal
├── ⚙️ links.json          # Configuración (perfil, enlaces, tema)
├── 🎨 input.css           # Archivo fuente Tailwind
├── 📦 output.css          # CSS compilado (auto-generado)
├── 🖼️ assets/             # Recursos multimedia
│   └── image.webp         # Imagen de perfil
├── 📋 package.json        # Dependencias del proyecto
├── 🔒 package-lock.json   # Lockfile de dependencias
└── 📖 README.md           # Documentación

```

## 🌐 Opciones de Despliegue

### GitHub Pages
1. Sube tu repo a GitHub
2. Ve a Settings → Pages
3. Selecciona la rama principal
4. ¡Tu sitio estará en `usuario.github.io/my-links`!

### Netlify (Recomendado)
1. Conecta tu repositorio de GitHub
2. Build command: `npm run build`
3. Publish directory: `./`
4. Deploy automático en cada push

### Vercel
1. Importa desde GitHub
2. Configuración automática detectada
3. Deploy instantáneo

### Hosting Tradicional
- Sube todos los archivos por FTP
- Asegúrate de incluir `output.css` compilado

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar el proyecto:

1. **Fork** el repositorio
2. **Crea** una rama: `git checkout -b feature/nueva-funcion`
3. **Commit** tus cambios: `git commit -m 'Añadir nueva función'`
4. **Push** a la rama: `git push origin feature/nueva-funcion`
5. **Abre** un Pull Request

### 🐛 Reportar Bugs
- Usa el sistema de [Issues de GitHub](https://github.com/galaterro/my-links/issues)
- Incluye capturas de pantalla si es posible
- Describe los pasos para reproducir el problema

## 🎯 Roadmap

- [ ] 🌓 Modo oscuro/claro automático
- [ ] 📊 Analytics de clics integrado
- [ ] 🎭 Más animaciones y transiciones
- [ ] 📱 PWA (Progressive Web App)
- [ ] 🔧 Panel de administración web
- [ ] 🌍 Internacionalización (i18n)

## 📜 Licencia

Este proyecto está bajo la **Licencia ISC** - consulta el archivo [LICENSE](LICENSE) para más detalles.

---

## 👨‍💻 Créditos

**Desarrollado por [@Galaterro](https://github.com/galaterro)** con la colaboración de **Claude Sonnet**.

### 🙏 Agradecimientos

- [Tailwind CSS](https://tailwindcss.com/) - Framework CSS
- [Google Fonts](https://fonts.google.com/) - Tipografía Inter
- [Bootstrap Icons](https://icons.getbootstrap.com/) - Iconografía

---

<div align="center">

**⭐ Si te gusta este proyecto, ¡dale una estrella! ⭐**

[🌐 Demo en Vivo](https://galaterro.github.io/my-links) • [🐛 Reportar Bug](https://github.com/galaterro/my-links/issues) • [💡 Solicitar Feature](https://github.com/galaterro/my-links/issues)

</div>