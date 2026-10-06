# CC-vtd

Sistema de transcripción de conversaciones de voz orientado a
mejorar la accesibilidad de personas con dificultades auditivas.
Discord será la plataforma de integración.

## Problema

Las conversaciones exclusivamente por voz pueden dificultar la
participación de personas con dificultades auditivas e incluso sordera. 
El proyecto permitirá seguir estas conversaciones mediante texto e identificar qué participante está hablando.

## Usuarios objetivo

- Personas con dificultades auditivas que utilizan Discord.

## Alcance del MVP

- Iniciar y detener una sesión de transcripción mediante comandos.
- Recibir audio de un canal de voz.
- Transcribirlo por fragmentos.
- Publicar el texto y el nombre del hablante en un canal de texto.
- Mantener temporalmente el estado de las sesiones.

Quedan fuera del MVP la traducción, los resúmenes, el panel web
y la integración con otras plataformas.

## Arquitectura inicial

- discord-service: gestiona la integración, recibe audio y publica texto.
- transcription-service: convierte los fragmentos de audio en texto.
- Persistencia o caché: conserva el estado temporal de las sesiones.

Las tecnologías y los protocolos están pendientes de validación.