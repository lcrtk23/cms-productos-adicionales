# Cards Interface - Figma Design Implementation

Una implementación completa de una interfaz de cards responsive basada en diseños de Figma, con soporte para desktop y mobile.

## 🎨 Características

### Desktop
- **Layout de 2 columnas** con cards lado a lado
- **Dimensiones exactas** según Figma (343px de ancho)
- **Sombras sutiles** para profundidad visual
- **Efectos hover** con transiciones suaves

### Mobile
- **Layout vertical** con cards apiladas
- **Ancho adaptativo** con máximo de 280px
- **Misma estructura** que desktop pero optimizada para móvil

### Componentes
- **Cards con imagen** y overlay de badge
- **Títulos** en mayúsculas con tipografía Averta
- **Detalles con bullets** (•) para mejor legibilidad
- **Botones "Ver más"** con flechas direccionales
- **Sidebars modales** con información detallada del producto
- **Footer con precio** y botón de compra

## 🛠️ Tecnologías

- **HTML5** semántico
- **CSS3** con Flexbox y Grid
- **Responsive Design** con media queries
- **Sin dependencias** externas

## 🎯 Especificaciones del Diseño

### Tipografía
- **Fuente**: Averta
- **Pesos**: 400, 600, 700
- **Tamaños**: 12px, 14px, 16px, 20px, 24px
- **Letter-spacing**: 2% consistente

### Colores
- **Texto principal**: #121212
- **Texto secundario**: #262626
- **Acentos**: #024DDF (azul)
- **Fondo**: #FFFFFF
- **Fondo de página**: #FAFBFC

### Espaciado
- **Padding de cards**: 16px 24px 8px (título), 12px 16px (detalles), 12px 24px (footer)
- **Gap entre elementos**: 4px, 8px, 12px, 16px, 24px
- **Border-radius**: 4px, 12px

## 📱 Responsive Breakpoints

- **Desktop**: > 750px (2 columnas)
- **Tablet**: ≤ 750px (1 columna centrada)
- **Mobile**: ≤ 768px (vista móvil optimizada)

## 🚀 Instalación y Uso

1. **Clonar el repositorio**:
   ```bash
   git clone https://github.com/lcrtk23/cards-interface.git
   ```

2. **Navegar al directorio**:
   ```bash
   cd cards-interface
   ```

3. **Servir localmente**:
   ```bash
   python3 -m http.server 5173
   ```

4. **Abrir en navegador**:
   ```
   http://localhost:5173
   ```

## 📁 Estructura del Proyecto

```
cards-interface/
├── index.html              # Archivo principal con HTML y CSS
├── DOCUMENTACION-TICKET-INTERFACE.md  # Documentación técnica
└── README.md               # Este archivo
```

## 🎨 Diseño Figma

El diseño está basado en especificaciones exactas de Figma:
- **Desktop**: node-id=2-516
- **Mobile**: node-id=3-2914
- **Product Header**: node-id=3-3579
- **Sidebar Footer Desktop**: node-id=3-3603
- **Sidebar Footer Mobile**: node-id=3-3907

## ✨ Características Implementadas

- ✅ **Diseño 1:1** con Figma
- ✅ **Responsive** completo
- ✅ **Accesibilidad** con semántica HTML
- ✅ **Performance** optimizada
- ✅ **Cross-browser** compatible
- ✅ **Hover effects** suaves
- ✅ **Modales** funcionales
- ✅ **Tipografía** exacta
- ✅ **Espaciado** preciso
- ✅ **Colores** consistentes

## 📄 Licencia

Este proyecto es privado y está bajo la propiedad de lcrtk23.

## 👥 Contribuciones

Este es un proyecto privado. Para colaboraciones, contactar al propietario.

---

**Desarrollado con ❤️ siguiendo las mejores prácticas de desarrollo web**
