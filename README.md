# NOVA AI

Asistente de voz personal tipo JARVIS para Windows — interfaz holográfica, pipeline completo de voz y memoria persistente.

## Características

- **Núcleo holográfico** con 3 estilos visuales (Quantum Core, Synapse Sphere, Arc Reactor) renderizado por código
- **Voz completa**: Whisper (Groq) → Llama 3.3 70B → Edge TTS neuronal en español
- **Modo manos libres** con wake word «Hey Nova» y detección de silencio local (VAD)
- **Memoria persistente**: recuerda datos entre sesiones («recuerda que...», «qué recuerdas»)
- **Recordatorios por voz** con aviso hablado a la hora programada
- **Herramientas del sistema**: abrir apps, carpetas, URLs, búsquedas, volumen, captura, procesos, matemática
- **Confirmación obligatoria** para acciones peligrosas (apagado)
- **Modo flotante** siempre encima + bandeja del sistema
- **Dashboard completo**: conversaciones, comandos, memoria, automatizaciones, diagnóstico y configuración

## Stack

C# / .NET 10 · Avalonia UI 12 · MVVM (CommunityToolkit) · NAudio · Groq API

## Instalación

1. Descarga el ejecutable de la sección Releases
2. Crea 
ova.json junto al exe:

\\\json
{
  " groqApiKey\: \gsk_TU_API_KEY\,
 \ttsVoice\: \es-MX-JorgeNeural\,
 \assistantName\: \Nova\
}
\\\

3. Ejecuta Nova.Desktop.exe

> Obtén tu API key gratis en https://console.groq.com

## Versiones

| Versión | Estado | Descripción |
|---|---|---|
| v0.4.0-alpha | Alpha | Dashboard holográfico, voz completa, memoria, recordatorios, manos libres, confirmaciones |
| v0.5.0-alpha | Alpha | Archivos (leer/escribir/borrar/mover/buscar), visión de pantalla, TTS ElevenLabs seleccionable, VAD adaptativo, wake word mejorado |
| v0.6.0-alpha | Alpha | Motor TTS propio Piper local con voz daniela, ElevenLabs eliminado, fallback multi-motor |

El código fuente es privado. Este repositorio aloja documentación y releases públicas.
