# Sistema de Cancelaciones Berel

Un sistema interactivo para consultar códigos y procedimientos de cancelación en el sistema Berel.

## 🚀 Características

- **Búsqueda Inteligente**: Busca cancelaciones por código o descripción
- **Filtros Avanzados**: 
  - **Todos**: Muestra todas las cancelaciones
  - **Error**: Filtra cancelaciones relacionadas con errores
  - **Cliente**: Muestra cancelaciones relacionadas con clientes
  - **Otros**: Cancelaciones que no son de error ni cliente
  - **Favoritos**: Guarda tus cancelaciones más utilizadas
- **Sistema de Favoritos**: Marca con estrella las cancelaciones que uses frecuentemente
- **Sistema de Usuarios**: Inicia sesión con un ID único para sincronizar favoritos entre dispositivos
- **Navegación por Etapas**: Selecciona la etapa específica del proceso
- **Información Completa**: Muestra código, descripción, procedimientos y observaciones

## 🛠️ Tecnología

- HTML5 puro
- CSS3 con diseño responsivo
- JavaScript vanilla (sin dependencias)
- LocalStorage para persistir favoritos
- Font Awesome para iconos

## 📱 Uso

### Navegación Principal

1. **Pantalla Principal**: Busca o filtra las cancelaciones
2. **Selección de Etapa**: Elige la etapa del proceso (Prefactura, Factura, etc.)
3. **Resultados**: Visualiza toda la información de la cancelación seleccionada

### Sistema de Usuarios

1. **Iniciar Sesión**: Haz clic en el botón "Iniciar Sesión" en la esquina superior derecha
2. **ID de Usuario**: Ingresa un ID único (ej: juan123, maria_ventas, etc.)
3. **Sincronización**: Tus favoritos se guardan con tu ID de usuario
4. **Acceso Multi-dispositivo**: Usa el mismo ID en cualquier dispositivo para acceder a tus favoritos
5. **Cerrar Sesión**: Haz clic en el ícono rojo para volver a favoritos locales

### Detalles de la Pantalla de Resultados

La pantalla de resultados muestra la información completa organizada en secciones:

- **Código**: Código único de la cancelación (ej. MDC00001) con estilo distintivo
- **Descripción**: Descripción completa del tipo de cancelación
- **Etapa**: Etapa seleccionada del proceso
- **Motivos de Cancelación**: Motivos SAT aplicables (resaltados en verde sólido)
- **Procedimiento**: Instrucciones claramente separadas:
  - **Tienda**: Acciones para el personal de tienda (etiqueta azul)
  - **Oficina**: Acciones para el personal de oficina (etiqueta azul)
- **Periodicidad**: Tiempo típico de procesamiento
- **Aplicación de Sustitución**: Si aplica o no
- **Observaciones Especiales**: Notas importantes con fondo naranja y ícono de advertencia

## 🌐 Acceso

El sistema está disponible en: https://4xguy.github.io/berel-cancelaciones/

## 📊 Estructura de Datos

Cada cancelación contiene:
```javascript
{
    code: "MDC00001",
    description: "ERROR EN DESCUENTO",
    stages: ["Otro Documento"],
    motivos: ["01"],
    procedure: "Tienda: ... Oficina: ...",
    periodicidad: "Generalmente, mismo día",
    aplicaSustitucion: "No",
    observaciones: "..."
}
```

## 🔧 Desarrollo Local

Para ejecutar localmente:
1. Clona el repositorio
2. Abre `index.html` en tu navegador
3. No requiere servidor web ni instalación

## 📝 Notas

- Los favoritos se guardan localmente en el navegador
- Con el sistema de usuarios, los favoritos se sincronizan entre dispositivos usando el mismo ID
- No se requiere contraseña, solo un ID único memorable
- El sistema funciona completamente offline una vez cargado
- Optimizado para dispositivos móviles y tablets
- Diseño con colores sólidos y alto contraste para mejor legibilidad

## 🔐 Privacidad

- Todos los datos se almacenan localmente en el navegador (localStorage)
- No se envía información a servidores externos
- Los IDs de usuario son solo para identificación local
- Cada usuario tiene su propio conjunto de favoritos independiente