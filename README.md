# 🚀 Portfolio Cristian Murcia - Senior Full-Stack Developer

Portfolio profesional moderno, responsive y con modo oscuro construido con HTML5, CSS3 y JavaScript vanilla.

## ✨ Características

- 🎨 **Diseño Moderno y Limpio**: Interfaz profesional con gradientes y animaciones suaves
- 🌓 **Dark Mode**: Alternancia entre modo claro y oscuro con persistencia en localStorage
- 📱 **Totalmente Responsive**: Optimizado para desktop, tablet y móviles
- ⚡ **Performance Optimizado**: Código ligero sin dependencias de frameworks
- 🎭 **Animaciones Suaves**: Transiciones y efectos visuales sutiles
- ♿ **Accesible**: Cumple con estándares de accesibilidad web
- 🎯 **SEO Optimizado**: Meta tags y estructura semántica

## 📂 Estructura del Proyecto

```
portfolio/
├── index.html          # Página principal
├── styles.css          # Estilos CSS
├── script.js           # Funcionalidad JavaScript
└── README.md           # Documentación
```

## 🎨 Secciones del Portfolio

1. **Hero/Inicio**: Presentación con animación de texto y enlaces principales
2. **Sobre Mí**: Biografía profesional con estadísticas destacadas
3. **Habilidades**: Tecnologías organizadas por categorías con barras de progreso
4. **Proyectos**: Grid de proyectos destacados con detalles y enlaces
5. **Experiencia**: Timeline con historial laboral y logros
6. **Contacto**: Formulario de contacto e información de contacto
7. **Footer**: Links adicionales y redes sociales

## 🛠️ Personalización

### 1. Información Personal

Edita el archivo `index.html` y reemplaza:

```html
<!-- Tu información -->
<h1 class="hero-title">Tu Nombre</h1>
<h2 class="hero-subtitle">Tu Título Profesional</h2>

<!-- Links de contacto -->
<a href="mailto:tu-email@gmail.com">...</a>
<a href="tel:+57tutelefono">...</a>

<!-- Links de redes sociales -->
<a href="https://github.com/tu-usuario">...</a>
<a href="https://linkedin.com/in/tu-perfil">...</a>
```

### 2. Colores y Temas

Edita las variables CSS en `styles.css`:

```css
:root {
    --primary-color: #3B82F6;        /* Color principal */
    --secondary-color: #8B5CF6;      /* Color secundario */
    --accent-color: #10B981;         /* Color de acento */
    /* ... más colores */
}
```

### 3. Proyectos

Agrega o edita proyectos en la sección `projects`:

```html
<article class="project-card">
    <div class="project-header">
        <span class="project-badge">Estado</span>
        <div class="project-links">
            <a href="tu-github-url" target="_blank">
                <i class="fab fa-github"></i>
            </a>
        </div>
    </div>
    <div class="project-content">
        <h3 class="project-title">Nombre del Proyecto</h3>
        <p class="project-description">Descripción...</p>
        <!-- Más contenido -->
    </div>
</article>
```

### 4. Experiencia Laboral

Edita la timeline en la sección `experience`:

```html
<div class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
        <h3>Tu Cargo</h3>
        <div class="timeline-company">Nombre Empresa</div>
        <!-- Más contenido -->
    </div>
</div>
```

### 5. Habilidades

Actualiza las barras de habilidades ajustando el `width` del `.skill-level`:

```html
<div class="skill-item">
    <span class="skill-name">Tecnología</span>
    <div class="skill-bar">
        <!-- Ajusta el width: 95%, 90%, 85%, etc. -->
        <div class="skill-level" style="width: 95%"></div>
    </div>
</div>
```

## 🚀 Cómo Usar

### Opción 1: Local

1. **Descarga los archivos** o clona el repositorio
2. **Abre `index.html`** en tu navegador
3. ¡Listo! El portfolio ya funciona localmente

### Opción 2: Hosting Gratuito

#### GitHub Pages

1. Crea un repositorio llamado `tu-usuario.github.io`
2. Sube los archivos
3. Ve a Settings → Pages
4. Selecciona la rama `main` y guarda
5. Tu portfolio estará en `https://tu-usuario.github.io`

#### Netlify

1. Arrastra la carpeta del portfolio a [netlify.com/drop](https://netlify.com/drop)
2. ¡Listo! Tu portfolio está online

#### Vercel

1. Instala Vercel CLI: `npm i -g vercel`
2. En la carpeta del proyecto: `vercel`
3. Sigue las instrucciones

### Opción 3: Hosting con Dominio Propio

1. Compra un dominio (ej: cristianmurcia.dev)
2. Usa cualquier hosting (Netlify, Vercel, Hostinger, etc.)
3. Conecta tu dominio siguiendo las instrucciones del hosting

## 📝 Funcionalidades JavaScript

### Dark Mode

```javascript
// El tema se guarda automáticamente en localStorage
// Los usuarios verán el último tema que eligieron
```

### Navegación Suave

```javascript
// Scroll suave a las secciones
// Resaltado automático del link activo
// Menú móvil responsive
```

### Animaciones

```javascript
// Animaciones al scroll usando Intersection Observer
// Contador animado para estadísticas
// Efectos hover en tarjetas de proyectos
// Typing animation en el hero
```

### Formulario de Contacto

```javascript
// Por defecto abre el cliente de email
// Puedes integrarlo con:
// - EmailJS (gratis): https://www.emailjs.com/
// - Formspree (gratis): https://formspree.io/
// - Tu propio backend
```

## 🎨 Personalización Avanzada

### Agregar Nuevas Secciones

1. Crea la sección en HTML:
```html
<section id="nueva-seccion" class="nueva-seccion">
    <div class="container">
        <h2 class="section-title">Título</h2>
        <!-- Contenido -->
    </div>
</section>
```

2. Agrega el link en la navegación:
```html
<li><a href="#nueva-seccion" class="nav-link">Nueva Sección</a></li>
```

3. Agrega estilos en CSS:
```css
.nueva-seccion {
    padding: var(--spacing-3xl) 0;
    /* Tus estilos */
}
```

### Cambiar Fuentes

1. Ve a [Google Fonts](https://fonts.google.com/)
2. Selecciona una fuente
3. Reemplaza en el `<head>` de `index.html`:
```html
<link href="https://fonts.googleapis.com/css2?family=TuFuente:wght@300;400;600;700&display=swap" rel="stylesheet">
```
4. Actualiza en CSS:
```css
:root {
    --font-primary: 'TuFuente', sans-serif;
}
```

### Agregar Google Analytics

Agrega antes del cierre de `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=TU-ID"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'TU-ID');
</script>
```

## 🐛 Solución de Problemas

### Los iconos no aparecen

Verifica que la conexión a Font Awesome esté activa:
```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
```

### El menú móvil no funciona

Asegúrate de que `script.js` esté correctamente vinculado:
```html
<script src="script.js"></script>
```

### Las animaciones no funcionan

Verifica que tu navegador soporte Intersection Observer (todos los navegadores modernos lo soportan)

## 📱 Integración con Servicios

### EmailJS (Formulario de Contacto)

1. Crea cuenta en [EmailJS](https://www.emailjs.com/)
2. Configura un servicio de email
3. Reemplaza en `script.js`:

```javascript
emailjs.send('tu_servicio_id', 'tu_template_id', formData)
    .then(() => {
        alert('¡Mensaje enviado!');
    });
```

### Google Analytics

Agrega tu ID de seguimiento como se mostró arriba.

### Vercel Analytics

Si usas Vercel, agrega:
```html
<script defer src="https://cdn.vercel-insights.com/v1/script.js"></script>
```

## 🎯 SEO Tips

1. **Actualiza los meta tags**:
```html
<meta name="description" content="Tu descripción">
<meta name="keywords" content="tus, palabras, clave">
```

2. **Agrega Open Graph**:
```html
<meta property="og:image" content="url-imagen-preview">
<meta property="og:url" content="tu-url">
```

3. **Sitemap**: Genera uno en [xml-sitemaps.com](https://www.xml-sitemaps.com/)

4. **robots.txt**:
```
User-agent: *
Allow: /
Sitemap: https://tu-dominio.com/sitemap.xml
```

## 📊 Performance Tips

1. **Optimiza imágenes**: Usa WebP cuando sea posible
2. **Minifica archivos**: Usa herramientas como [minifier.org](https://www.minifier.org/)
3. **Lazy loading**: Para imágenes grandes
4. **CDN**: Usa Cloudflare para archivos estáticos

## 🤝 Contribuciones

¿Encontraste un bug o tienes una mejora? ¡Abre un issue o envía un PR!

## 📄 Licencia

Este proyecto es de código abierto. Siéntete libre de usarlo y modificarlo para tu propio portfolio.

## 🎉 Easter Eggs

- Intenta el Konami Code: ↑ ↑ ↓ ↓ ← → ← → B A
- Abre la consola del navegador para ver un mensaje especial 😉

## 📞 Contacto

**Cristian Murcia**
- Email: cristian.murcia175@gmail.com
- GitHub: [github.com/cristian-murcia](https://github.com/cristian-murcia)
- LinkedIn: [linkedin.com/in/cristian-murcia-dev](https://linkedin.com/in/cristian-murcia-dev)

---

**Hecho con ❤️ y mucho ☕ por Cristian Murcia**

⭐ Si te gustó este portfolio, dale una estrella al repositorio!
