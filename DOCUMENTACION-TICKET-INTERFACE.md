# Documentación - Ticket Interface CSS Only

## Descripción General
Este archivo HTML implementa una interfaz de tickets completamente funcional utilizando únicamente HTML y CSS, sin JavaScript. La interfaz permite mostrar productos adicionales como FAST PASS y PAQUETE VIP con paneles deslizantes de información detallada.

## Estructura del Proyecto

### Archivo Principal
- **index.html** - Interfaz completa de tickets con estilos integrados

### Características Principales
- ✅ **Responsive Design** - Adaptable a desktop y móvil
- ✅ **CSS Only** - Sin dependencias de JavaScript
- ✅ **Paneles Deslizantes** - Usando técnicas CSS con `:target`
- ✅ **Doble Vista** - Desktop y móvil con diferentes layouts
- ✅ **Integración con Ticketmaster** - Logos y enlaces funcionales

## Estructura de Componentes

### 1. Container Principal (`tmpe-container`)
```css
.tmpe-container {
  width: 800px;
  max-width: 800px;
  background: #FAFBFC;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.15);
}
```

### 2. Tickets Items
Cada ticket contiene:
- **Logo del canal** (`tmpe-logo-container`)
- **Información del producto** (`tmpe-info-container`)
- **Botón de acción** (`tmpe-link-details` / `tmpe-link-mobile`)

### 3. Sistema de Paneles Modales
Utiliza la técnica CSS `:target` para mostrar/ocultar paneles:
```css
#tmpe-toggle-1:target ~ .tmpe-overlay-1 {
  opacity: 1;
  visibility: visible;
}
```

## Productos Configurados

### FAST PASS
- **Precio**: S/30.80
- **Descripción**: Adicionalo a la compra de tu entrada
- **Incluye**:
  - 1 entrada Platinum
  - Acceso VIP Lounge
  - Aperitivos y bebidas (2 fichas)
  - Regalo VIP exclusivo
  - Merchandising exclusivo
  - Acceso anticipado al estadio

### PAQUETE VIP
- **Precio**: S/30.80
- **Descripción**: Incluye entrada platinium
- **Incluye**: Mismo contenido que FAST PASS

## Responsive Design

### Desktop (>768px)
- Layout horizontal con botones de "Más Información"
- Efectos hover en tickets y botones
- Ancho fijo de 800px

### Móvil (≤768px)
- Layout vertical optimizado para touch
- Botones circulares de navegación
- Ancho completo del viewport
- Ajustes tipográficos específicos

## Paleta de Colores

### Colores Principales
- **Azul Principal**: `#024DDF` - Botones y enlaces
- **Azul Hover**: `#0035A0` - Estados activos
- **Fondo Principal**: `#FAFBFC`
- **Texto Principal**: `#262626`
- **Texto Secundario**: `#7D7D7D`
- **Bordes**: `#D6D6D6`

### Colores de Estado
- **Disponible**: `#048851` (verde)
- **Próximamente**: `#646464` (gris)

## Tipografía
- **Familia Principal**: 'Averta', 'Helvetica Neue', Helvetica, Arial, sans-serif
- **Títulos**: 20px, weight 700
- **Subtítulos**: 16px, weight 400
- **Badges**: 12px, weight 600, uppercase
- **Botones**: 16px, weight 600

## Funcionalidades CSS

### Paneles Deslizantes
```css
.tmpe-sidebar-panel {
  transform: translateX(100%);
  transition: transform 0.3s ease;
}

#tmpe-toggle-1:target ~ .tmpe-overlay-1 .tmpe-sidebar-panel {
  transform: translateX(0);
}
```

### Efectos Hover
- Cambio de fondo en tickets
- Inversión de colores en botones
- Transiciones suaves (0.2s ease)

### Media Queries
- Punto de quiebre: 768px
- Ajustes específicos para móvil y desktop

## Enlaces y Recursos

### Imágenes Externas
- **Logo Ticketmaster**: `https://prod-assets.tmlat.com/T_9318699a9f.svg`
- **Imagen del Producto**: `https://prod-assets.tmlat.com/image_15cd533576.png`

### Enlaces de Compra
- **URL Base**: `https://www.ticketmaster.pe/event/la-tarumba-lima-563-temporada-2025-venta-cupn-empresa`

## Consideraciones Técnicas

### Ventajas
- Sin dependencias de JavaScript
- Carga rápida y ligera
- SEO friendly
- Accesibilidad mejorada

### Limitaciones
- Funcionalidad limitada comparado con JavaScript
- Dificultad para animaciones complejas
- Dependencia de técnicas CSS específicas

## Uso e Implementación

### Para Integrar:
1. Copiar el código HTML completo
2. Ajustar URLs de imágenes según necesidad
3. Modificar enlaces de compra
4. Personalizar colores y tipografías según marca

### Para Personalizar:
- Modificar variables de color en el CSS
- Ajustar dimensiones de componentes
- Cambiar contenido de productos
- Adaptar responsive breakpoints

## Mantenimiento
- Verificar enlaces externos periódicamente
- Actualizar precios según sea necesario
- Testear en diferentes navegadores y dispositivos
- Validar accesibilidad web