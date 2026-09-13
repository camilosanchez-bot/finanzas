# 💰 Money-Flow Retirement Planner

**Tu app personal para planificar tu retiro usando el método Money-Flow de Claudia Uribe**

## 📋 Contenido

Este proyecto contiene una aplicación web completa para gestionar tu plan de retiro con:

- **Calculadora de Número Dorado**: El patrimonio necesario para vivir hasta los 85 años
- **Las 3 Palancas del Método Money-Flow**:
  - Palanca 1: Cómo ordenar tu dinero
  - Palanca 2: Rentar mejor según tu perfil de inversión
  - Palanca 3: Método Vortex (3 fondos rentables)
- **Seguimiento de inversiones**: Registra tus aportes mensuales
- **Proyecciones financieras**: Visualiza gráficos de crecimiento
- **Almacenamiento local**: Tus datos se guardan en tu navegador

## 🚀 Instalación y Uso

### Opción 1: Con Node.js (Recomendado)

#### Requisitos:
- Node.js 16+ ([Descargar](https://nodejs.org/))
- npm (viene con Node.js)

#### Pasos:

1. **Abre una terminal** en la carpeta del proyecto

2. **Instala las dependencias**:
```bash
npm install
```

3. **Inicia el servidor de desarrollo**:
```bash
npm run dev
```

4. **Abre tu navegador** en `http://localhost:3000`

La app se abrirá automáticamente.

### Opción 2: Sin Node.js (Alternativa simple)

Si no quieres instalar Node.js, puedes usar la versión HTML stand-alone:

1. Crea un archivo llamado `standalone.html` en tu computadora
2. Copia todo el código de abajo
3. Guárdalo
4. Haz doble clic para abrirlo en tu navegador

```html
[Ver archivo standalone.html incluido en la carpeta]
```

## 📁 Estructura del Proyecto

```
moneyflow-app/
├── main.jsx          # Código React de la app
├── style.css         # Estilos CSS
├── index.html        # Archivo HTML principal
├── vite.config.js    # Configuración de Vite
├── package.json      # Dependencias del proyecto
└── README.md         # Este archivo
```

## 🎯 Cómo usar la app

### 1. Setup Inicial
Ingresa tus datos personales y financieros:
- Tu nombre
- Gasto mensual actual
- Años para alcanzar retiro
- Capital ya invertido
- Patrimonio actual (bienes a vender)
- Rentabilidad esperada
- Inflación esperada

### 2. Dashboard
Verás tu **Número Dorado** y métricas clave, más botones para explorar:
- Las 3 Palancas
- Mi Seguimiento
- Proyecciones

### 3. Las 3 Palancas
Entiende la estrategia Money-Flow:
- **Palanca 1**: Cómo ordenar tu dinero (aporte primero)
- **Palanca 2**: Distribución de inversión tipo "casa" (Paredes, Habitaciones, Terraza, Piscina)
- **Palanca 3**: Método Vortex (Fondo de Imprevistos, Reserva de Oxígeno, Fondo de Retiro)

### 4. Mi Seguimiento
Registra mes a mes tus aportes para ver cómo avanzas hacia tu meta.

### 5. Proyecciones
Visualiza gráficos de crecimiento y hitos importantes.

## 💾 Datos Guardados

Tu información se almacena localmente en tu navegador usando `localStorage`. 
- **No se envía a Internet**
- **Solo tú ves tus datos**
- **Persisten entre sesiones**

Si quieres limpiar los datos, abre las herramientas de desarrollador (F12) y ejecuta:
```javascript
localStorage.removeItem('moneyflow_profile');
```

## 🔧 Tecnologías Usadas

- **React 18**: Framework de UI
- **Vite**: Bundler y servidor de desarrollo
- **Recharts**: Gráficos interactivos
- **CSS Puro**: Diseño responsivo

## 📊 Fórmulas Utilizadas

### Número Dorado
```
Gasto Retiro Mensual = Gasto Actual × (1 + Inflación)^Años
Dinero Necesario Hoy = (Gasto Retiro × 12 × 30 años) / (1 + Rentabilidad)^Años
```

### Proyección de Patrimonio
```
Balance = Capital Inicial + Aportes Mensuales
Rentabilidad = Balance × (1 + Tasa Mensual)^Meses
```

## 🆘 Solución de Problemas

### La app no carga
- Verifica que tengas Node.js instalado: `node --version`
- Intenta eliminar la carpeta `node_modules` y `package-lock.json`, luego `npm install` de nuevo

### Los datos no se guardan
- Verifica que el navegador no tenga localStorage deshabilitado
- Intenta en modo no privado/incógnito

### Gráficos no se muestran
- Actualiza la página (F5 o Ctrl+R)
- Verifica que tu navegador no tenga bloqueadores de contenido

## 📈 Personalización

Para modificar la app:

1. **Cambiar colores**: Edita `style.css` y busca los valores hexadecimales (ej: `#378ADD`)
2. **Cambiar textos**: Edita los strings en `main.jsx`
3. **Agregar funcionalidades**: Modifica `main.jsx` y agrega lógica React

## 🚀 Deployment (Subir a Internet)

Si quieres una URL pública:

### Con Vercel (Recomendado - Gratis):
1. Crea cuenta en [vercel.com](https://vercel.com)
2. Conecta tu repositorio de GitHub
3. Vercel despliega automáticamente

### Con Netlify (También Gratis):
1. Crea cuenta en [netlify.com](https://netlify.com)
2. Conecta tu repositorio o arrastra la carpeta `dist`
3. Listo, tendrás una URL pública

## 📞 Soporte

Si encuentras problemas:
1. Revisa la sección "Solución de Problemas" arriba
2. Asegúrate de tener Node.js 16+ instalado
3. Intenta en otro navegador

## 📝 Notas Importantes

- **Los números son estimados**: Consulta con un asesor financiero real antes de tomar decisiones
- **Actualiza regularmente**: Ingresa nuevos aportes mensualmente para ver tu progreso real
- **Revisa el plan anualmente**: Las condiciones de mercado cambian

## 🎓 Más Información sobre Money-Flow

Este método fue enseñado por **Claudia Uribe**, analista financiera.
Para información oficial, busca sus masterclasses y contenido.

---

**¡Que disfrutes tu app! 🚀💰**

Recuerda: No es lo que ganas, es lo que tu dinero genera cada mes.
