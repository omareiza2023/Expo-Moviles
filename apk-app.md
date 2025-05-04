# Paso a paso para crear una app con Ionic, Angular y Capacitor (Android)

# 1. Tener instalado Node.js

# 2. Tener instalado npm (viene con Node.js)

# 3. Instalar Angular CLI
npm install -g @angular/cli

# 4. Instalar Ionic CLI, native-run y cordova-res
npm install -g @ionic/cli native-run cordova-res

# 5. Crear una aplicación con Ionic y Angular
ionic start photo-gallery tabs --type=angular --capacitor

# 6. Ir a la carpeta del proyecto
cd photo-gallery

# 7. Instalar los plugins necesarios para funcionalidad nativa
npm install @capacitor/camera @capacitor/preferences @capacitor/filesystem

# 8. Correr la aplicación en el navegador (modo desarrollo)
ionic serve

# 9. Instalar el paquete de Capacitor para Android
npm install @capacitor/android

# 10. Agregar la plataforma Android al proyecto
npx cap add android

# 11. Compilar la aplicación Angular
ionic build

# 12. Sincronizar el código con la plataforma Android
npx cap sync android

# 13. Instalar Android Studio (si no lo tienes ya instalado)

# 14. Abrir el proyecto Android en Android Studio
npx cap open android