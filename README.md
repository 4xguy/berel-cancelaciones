# Grupo Color - Portal de Aplicaciones

Portal de aplicaciones web para Grupo Color. Incluye herramientas y sistemas para optimizar procesos empresariales.

## 📖 Guía de Usuario - Sistema de Cancelaciones

### ¿Qué es el Sistema de Cancelaciones?
Es una herramienta que te ayuda a encontrar rápidamente los códigos y procedimientos correctos cuando necesitas cancelar una operación en el sistema Berel.

### 🏁 Cómo Empezar

1. **Entra al portal**: Visita https://gc.proceso.app
2. **Haz clic en "Sistema de Cancelaciones"**: Es la primera aplicación disponible
3. **Ya estás listo para buscar**: No necesitas instalar nada

### 📱 Paso a Paso para Buscar una Cancelación

#### Paso 1: Encuentra tu Cancelación
En la primera pantalla verás:
- **Una barra de búsqueda**: Escribe el código (como MDC00001) o palabras clave (como "descuento" o "precio")
- **Botones de filtro** en la parte superior:
  - 🔍 **Todos**: Ver todas las cancelaciones
  - ⚠️ **Error**: Solo cancelaciones por errores del sistema
  - 👤 **Cliente**: Solo cancelaciones solicitadas por clientes
  - 📋 **Otros**: Otras cancelaciones
  - ⭐ **Favoritos**: Tus cancelaciones guardadas
- **Lista de cancelaciones**: Cada una muestra su código y descripción

**Tip**: Puedes marcar como favorita cualquier cancelación haciendo clic en la estrella ⭐

#### Paso 2: Selecciona la Etapa
Después de elegir una cancelación, selecciona en qué etapa del proceso estás:
- Prefactura
- Factura
- Otro Documento
- Etc.

#### Paso 3: Ve el Procedimiento Completo
En la pantalla final encontrarás toda la información necesaria:
- **Código y descripción** de la cancelación
- **Motivos SAT** que debes usar (en verde)
- **Procedimientos** separados para:
  - 🏪 **Tienda**: Lo que debe hacer el personal de tienda
  - 🏢 **Oficina**: Lo que debe hacer el personal de oficina
- **Tiempo estimado** de resolución
- **Observaciones importantes** (en naranja si requieren atención especial)

### 👤 Sistema de Usuarios (Opcional)

Si usas frecuentemente el sistema, puedes crear una cuenta para guardar tus favoritos:

1. **Haz clic en el ícono de usuario** (arriba a la derecha)
2. **Crea tu cuenta**:
   - Elige un nombre de usuario (ejemplo: juan.perez)
   - Crea una contraseña
   - La primera vez que entres, tu cuenta se creará automáticamente
3. **Beneficios**:
   - Tus favoritos se guardan permanentemente
   - Puedes acceder desde cualquier dispositivo con tu usuario y contraseña
   - No perderás tus favoritos si cambias de computadora

### 💡 Consejos Útiles

- **Usa la búsqueda**: Es más rápido escribir palabras clave que buscar manualmente
- **Marca tus favoritos**: Si usas ciertas cancelaciones frecuentemente, márcalas con la estrella
- **Lee las observaciones**: El cuadro naranja contiene información importante
- **Navega fácilmente**: 
  - Botón 🏠 para volver al portal principal
  - Botón ← para regresar a la pantalla anterior
  - Botón "Nueva Consulta" para buscar otra cancelación

### ❓ Preguntas Frecuentes

**P: ¿Necesito instalar algo?**
R: No, funciona directamente en tu navegador (Chrome, Firefox, Safari, etc.)

**P: ¿Puedo usarlo en mi celular?**
R: Sí, está diseñado para funcionar en computadoras, tablets y celulares

**P: ¿Qué pasa si olvido mi contraseña?**
R: Contacta al administrador del sistema para asistencia

**P: ¿Mis favoritos se borran?**
R: Sin cuenta: Se guardan en tu navegador actual
Con cuenta: Se guardan permanentemente y puedes acceder desde cualquier dispositivo

**P: ¿Qué significan los colores?**
- **Morado**: Códigos de cancelación
- **Verde**: Motivos SAT aplicables
- **Azul**: Etiquetas de procedimientos (Tienda/Oficina)
- **Naranja**: Observaciones importantes
- **Amarillo**: Estrella de favoritos

## 🌐 Acceso

- Portal principal: https://gc.proceso.app
- Sistema de Cancelaciones: https://gc.proceso.app/cancelaciones

## 🛠️ Información Técnica

### Tecnologías Utilizadas
- HTML5 puro
- CSS3 con diseño responsivo
- JavaScript vanilla (sin dependencias)
- LocalStorage para persistir favoritos
- Font Awesome para iconos

### Estructura de Datos
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

### Desarrollo Local
Para ejecutar localmente:
1. Clona el repositorio
2. Abre `index.html` en tu navegador
3. No requiere servidor web ni instalación

### Notas Técnicas
- Los favoritos se guardan localmente en el navegador
- Con el sistema de usuarios, los favoritos se sincronizan entre dispositivos usando el mismo ID
- Sistema de autenticación simple con contraseña (hash almacenado localmente)
- El sistema funciona completamente offline una vez cargado
- Optimizado para dispositivos móviles y tablets
- Diseño con colores sólidos y alto contraste para mejor legibilidad

### Privacidad y Seguridad
- Todos los datos se almacenan localmente en el navegador (localStorage)
- No se envía información a servidores externos
- Las contraseñas se almacenan como hash simple (no como texto plano)
- Cada usuario tiene su propio conjunto de favoritos independiente
- **Nota**: Este es un sistema de seguridad básico apropiado para datos no sensibles