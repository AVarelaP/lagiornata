# La Giornata — Sitio Web

Medio de periodismo digital explicativo para Honduras y Centroamérica.

## Estructura

```
lagiornata/
├── index.html          # Página principal (home)
├── css/
│   └── style.css       # Estilos globales
└── pages/
    └── membresias.html # Página de membresías y suscripciones
```

## Deploy en GitHub Pages

1. Sube todos los archivos a un repositorio de GitHub
2. Ve a **Settings → Pages**
3. En "Source" selecciona **Deploy from a branch**
4. Selecciona la rama `main` y carpeta `/ (root)`
5. Guarda — tu sitio estará disponible en `https://[usuario].github.io/[repo]/`

## Personalización

### Cambiar colores
En `css/style.css`, modifica las variables CSS en `:root`:
- `--navy: #0B1F3A` → Azul editorial principal
- `--coral: #FF6B6B` → Acento coral (CTAs, destacados)
- `--beige: #F5F1EB` → Fondo secciones

### Agregar imágenes reales
Reemplaza los `div` con clase `ph-*` por elementos `<img>`:
```html
<img src="ruta/imagen.jpg" alt="Descripción" style="width:100%;height:100%;object-fit:cover">
```

### Integrar pasarela de pago real
En `pages/membresias.html`, reemplaza la función `processPayment()` por la integración con:
- **Stripe** (recomendado para tarjetas)
- **PayPal**
- **Tigo Money / BAC** (opciones locales Honduras)

## Fuentes externas utilizadas
- Google Fonts: Merriweather Sans + Playfair Display
- Sin dependencias de JavaScript externas

## Créditos
Diseñado siguiendo el Manual de Marca de La Giornata v1.0 — Grupo 4.
