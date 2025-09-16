# Claseds

Claseds es una aplicación móvil multiplataforma desarrollada con Flutter. El proyecto incluye soporte para Android, iOS, web y escritorios (macOS, Linux, Windows) y sigue la estructura estándar de proyectos Flutter.

## Resumen

- Lenguaje: Dart
- Framework: Flutter
- Punto de entrada: `lib/main.dart`

## Estructura principal

- `lib/` - Código fuente principal.
- `android/`, `ios/`, `macos/`, `linux/`, `windows/`, `web/` - Configuración por plataforma y código nativo cuando aplica.
- `build/` - Artefactos de compilación generados.
- `test/` - Pruebas unitarias y de widgets.
- `pubspec.yaml` - Dependencias y metadatos del proyecto.

## Requisitos previos

- Tener instalado Flutter en una versión compatible. Consulta https://flutter.dev/docs/get-started/install
- SDKs de plataforma según donde quieras compilar (Android SDK, Xcode para iOS/macOS).

## Instalación y ejecución

1. Clona el repositorio:

```bash
git clone https://github.com/ISCOUTB/claseds.git
cd claseds
```

2. Obtén las dependencias:

```bash
flutter pub get
```

3. Ejecuta la aplicación en un dispositivo/emulador:

```bash
flutter run
```

4. Ejecuta en web (si tienes Chrome):

```bash
flutter run -d chrome
```

5. Analizar y probar:

```bash
flutter analyze
flutter test
```

## Construcción de release

- Android (APK):

```bash
flutter build apk --release
```

- iOS (desde macOS):

```bash
flutter build ios --release
```

- Web:

```bash
flutter build web
```

## Buenas prácticas

- Mantén `pubspec.yaml` actualizado y corre `flutter pub get` tras cambios.
- Si agregas plugins nativos, ejecuta `pod install` en `ios/` cuando sea necesario.
- Añade pruebas en `test/` y corre `flutter analyze` en CI para detectar problemas tempranos.

## Notas específicas del proyecto

- El código fuente inicia en `lib/main.dart`. Revisa ese archivo para entender el flujo de la app.
- Archivos de configuración nativa están en sus respectivas carpetas (`android/`, `ios/`, etc.).

## Contacto

Si necesitas ayuda con este repositorio, abre un issue o contacta a los mantenedores.

---

Este archivo fue actualizado automáticamente para ofrecer una guía inicial en español; ajústalo según las necesidades del proyecto.
