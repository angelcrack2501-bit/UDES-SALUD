# UDES Salud · app Android (APK)

La app web (`index.html`) se empaqueta como app Android con **Capacitor**.

## Descargar el APK
GitHub → pestaña **Releases** → `UDES-Salud.apk`. En el celular: abrirlo y permitir "instalar apps desconocidas".
Cada cambio en `index.html` construye un APK nuevo solo (GitHub Actions).

## Abrirlo en Android Studio (para la clase)
1. Instala Node.js. En esta carpeta: `npm install` y luego `npm run sync`.
2. Android Studio → **Open** → carpeta `app-android/android`. Espera a que Gradle termine.
3. **Build → Build App Bundle(s) / APK(s) → Build APK(s)**. O dale ▶ con un celular conectado o un emulador.

## Cómo funciona
- `www/index.html`: copia de la app web.
- `capacitor.config.json`: nombre (UDES Salud) e id (`co.udes.salud`).
- `android/`: proyecto nativo de Android que muestra la app web en un WebView.
