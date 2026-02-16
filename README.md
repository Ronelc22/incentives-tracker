# Incentives Tracker Amstar - PWA

## 📱 Progressive Web App

Esta es la versión PWA (Progressive Web App) del sistema de seguimiento de incentivos para representantes de Amstar.

## ✨ Características

- ✅ **Instalable en Android/iOS** - Funciona como app nativa
- ✅ **Funciona Offline** - Accede a la app sin conexión a internet
- ✅ **Actualizaciones Automáticas** - Siempre tendrás la última versión
- ✅ **Rápida y Ligera** - Ocupa muy poco espacio
- ✅ **Sin Play Store** - Se instala directamente desde el navegador

## 🚀 Cómo Instalar en Android

### Opción 1: Desde Chrome (Recomendado)

1. Abre Google Chrome en tu teléfono Android
2. Visita la URL donde esté alojada la app
3. Presiona el menú (⋮) en la esquina superior derecha
4. Selecciona **"Agregar a pantalla de inicio"** o **"Instalar app"**
5. Confirma la instalación
6. ¡Listo! El icono aparecerá en tu pantalla de inicio

### Opción 2: Banner Automático

1. Abre la app en Chrome
2. Espera 3 segundos
3. Aparecerá un banner en la parte inferior
4. Presiona **"Instalar"**
5. ¡Listo!

## 🚀 Cómo Instalar en iOS (iPhone/iPad)

1. Abre Safari (debe ser Safari, no Chrome)
2. Visita la URL de la app
3. Presiona el botón de compartir (📤)
4. Desplázate hacia abajo y selecciona **"Agregar a pantalla de inicio"**
5. Confirma y presiona **"Agregar"**
6. ¡Listo!

## 🌐 Cómo Alojar la PWA

### Opción 1: GitHub Pages (Gratis y Fácil)

1. Crea un repositorio en GitHub
2. Sube todos los archivos de la carpeta `pwa/`
3. Ve a Settings → Pages
4. Selecciona la rama `main` como fuente
5. Guarda y espera unos minutos
6. Tu app estará disponible en: `https://tuusuario.github.io/nombre-repo/`

### Opción 2: Netlify/Vercel (Gratis)

1. Crea una cuenta en [Netlify](https://netlify.com) o [Vercel](https://vercel.com)
2. Arrastra la carpeta `pwa/` a su dashboard
3. Obtendrás una URL automáticamente
4. Comparte la URL con tu equipo

### Opción 3: Hosting Tradicional

1. Sube todos los archivos a tu servidor web
2. Asegúrate de que el servidor tenga HTTPS habilitado (requerido para PWAs)
3. Accede a través de tu dominio

## 📂 Estructura de Archivos

```
pwa/
├── index.html           # Archivo principal de la app
├── manifest.json        # Configuración de la PWA
├── service-worker.js    # Script para funcionalidad offline
├── icon-192.png         # Icono pequeño de la app
├── icon-512.png         # Icono grande de la app
└── README.md           # Este archivo
```

## 🔧 Características Técnicas

- **Framework**: React 18 (sin compilación necesaria)
- **Estilos**: Tailwind CSS
- **Iconos**: Lucide React
- **Storage**: LocalStorage (datos guardados en el dispositivo)
- **Offline**: Service Worker con cache estratégico
- **Tamaño**: ~500KB en total

## 🔒 Seguridad y Datos

- Todos los datos se guardan localmente en el dispositivo
- No se envía información a servidores externos
- Los datos son específicos por hotel y usuario
- Funciona completamente offline

## 🛠️ Personalización

### Cambiar Colores del Tema

Edita `manifest.json`:
```json
{
  "theme_color": "#2563eb",
  "background_color": "#2563eb"
}
```

### Cambiar Nombre de la App

Edita `manifest.json`:
```json
{
  "name": "Tu Nombre Personalizado",
  "short_name": "Nombre Corto"
}
```

### Cambiar Iconos

Reemplaza `icon-192.png` y `icon-512.png` con tus propios iconos.

## 📱 Requisitos

- **Android**: Chrome 80+ o Samsung Internet 11+
- **iOS**: Safari 11.3+
- **Desktop**: Chrome 80+, Edge 80+, Firefox 90+

## 🐛 Solución de Problemas

### La app no se instala

- Asegúrate de estar usando HTTPS (no HTTP)
- Verifica que el archivo `manifest.json` sea válido
- Limpia la caché del navegador

### Los datos no se guardan

- Verifica que el navegador permita LocalStorage
- No uses modo incógnito/privado
- Asegúrate de no limpiar los datos del navegador

### La app no funciona offline

- Espera a que se complete la primera carga
- Verifica que el Service Worker esté registrado
- Abre Chrome DevTools → Application → Service Workers

## 📞 Soporte

Para reportar problemas o sugerencias, contacta al equipo de desarrollo.

## 📄 Licencia

Uso interno de Amstar - Todos los derechos reservados.

---

¡Disfruta usando Incentives Tracker Amstar! 🎉
