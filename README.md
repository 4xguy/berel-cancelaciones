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
- **Navegación por Etapas**: Selecciona la etapa específica del proceso
- **Información Completa**: Muestra código, descripción, procedimientos y observaciones

## 🛠️ Tecnología

- HTML5 puro
- CSS3 con diseño responsivo
- JavaScript vanilla (sin dependencias)
- LocalStorage para persistir favoritos
- Font Awesome para iconos

## 📱 Uso

1. **Pantalla Principal**: Busca o filtra las cancelaciones
2. **Selección de Etapa**: Elige la etapa del proceso (Prefactura, Factura, etc.)
3. **Resultados**: Visualiza toda la información de la cancelación seleccionada

### Detalles de la Pantalla de Resultados

- **Código**: Código único de la cancelación (ej. MDC00001)
- **Descripción**: Descripción completa del tipo de cancelación
- **Etapa**: Etapa seleccionada del proceso
- **Motivos de Cancelación**: Motivos SAT aplicables (resaltados en verde)
- **Procedimiento**: Instrucciones separadas para Tienda y Oficina
- **Periodicidad**: Tiempo típico de procesamiento
- **Aplicación de Sustitución**: Si aplica o no
- **Observaciones Especiales**: Notas importantes (resaltadas con advertencia)

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
- El sistema funciona completamente offline una vez cargado
- Optimizado para dispositivos móviles y tablets