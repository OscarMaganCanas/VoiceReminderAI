# 🎙️ VoiceReminderAI

Aplicación Android para **crear recordatorios hablando**, sin necesidad de escribir. El usuario pulsa un botón, dicta su recordatorio y la app lo transcribe a texto usando el reconocimiento de voz del dispositivo.

> 🚧 **Proyecto en desarrollo.** Actualmente está implementada la funcionalidad de voz a texto. Consulta la [hoja de ruta](#️-hoja-de-ruta) para ver las próximas funcionalidades.

## 📱 Funcionalidades

- ✅ Reconocimiento de voz a texto con la API `RecognizerIntent` de Android
- ✅ Detección automática del idioma del dispositivo
- ✅ Muestra en pantalla el texto reconocido
- ✅ Gestión de errores si el dispositivo no soporta reconocimiento de voz

## 🛠️ Tecnologías

| | |
|---|---|
| **Lenguaje** | Java 11 |
| **Plataforma** | Android (SDK mínimo 26 · Android 8.0) |
| **Build** | Gradle (Kotlin DSL) |
| **UI** | XML Layouts · AppCompat · Material Components |
| **APIs** | Android Speech Recognition (`RecognizerIntent`) |

## 🗂️ Estructura del proyecto

```
app/src/main/
├── java/com/oscar/voicereminder/
│   └── MainActivity.java      # Lógica de captura y reconocimiento de voz
├── res/layout/
│   └── activity_main.xml      # Interfaz principal
└── AndroidManifest.xml
```

## 🚀 Cómo ejecutarlo

1. Clona el repositorio:
   ```bash
   git clone https://github.com/OscarMaganCanas/VoiceReminderAI.git
   ```
2. Ábrelo con **Android Studio**.
3. Espera a que Gradle sincronice las dependencias.
4. Ejecútalo en un dispositivo físico o emulador con **Android 8.0 o superior** y con los servicios de Google instalados (necesarios para el reconocimiento de voz).

## 🗺️ Hoja de ruta

- [x] Captura de voz y transcripción a texto
- [ ] Extraer fecha y hora del texto dictado (*"mañana a las 10, llamar al médico"*)
- [ ] Programar notificaciones con `AlarmManager`
- [ ] Guardar los recordatorios en una base de datos local (Room / SQLite)
- [ ] Listado de recordatorios con opción de editar y borrar
- [ ] Integración con IA para interpretar recordatorios en lenguaje natural

## 👤 Autor

**Óscar Magán Cañas** · [GitHub](https://github.com/OscarMaganCanas)
