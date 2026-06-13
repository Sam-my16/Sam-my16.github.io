---
title: "Fiebre mundialista"
categories:
  - Programación
tags:
  - Mundial 2026
  - Programación
  - Shortcuts Apple
  - Apple
---

Quiero estar al día con los partidos del mundial, pero buscar en Google cada vez me resulta molesto, y los posteos de Instagram desaparecen en el feed antes de que los pueda ver. Seguramente existe alguna app que resuelve esto, pero encontré motivación suficiente para hacerlo por mi cuenta.

Primero pensé en Python, pero la computadora tendría que estar prendida todo el tiempo — poco viable. El teléfono, en cambio, siempre está. Ahí fue cuando me acordé de **Shortcuts**, la app nativa de Apple.

Para obtener los datos usé [thesportsdb.com](https://www.thesportsdb.com/), una base de datos deportiva gratuita que incluye información del Mundial 2026. El principal obstáculo fue manejar las fechas: los horarios vienen en UTC y convertirlos a mi zona horaria dentro de Shortcuts no es exactamente elegante, pero encontré la manera.

El flujo quedó así:

1. Accede a la base de datos.
2. Obtiene todos los eventos del mundial.
3. Convierte la fecha de cada partido de UTC a la zona horaria usada en el teléfono.
4. Obtiene la fecha actual.
5. Si las fechas coinciden, registra el equipo local, el equipo visitante y la hora del partido.
6. Agrupa todos los partidos del día y envía una notificación con esa información. Gracias a la integración de WhatsApp con Shortcuts, también se puede mandar como mensaje de texto en lugar de notificación.

Con una pequeña variación en el paso 5, registrando goles en vez de hora, y comparando con el día anterior en lugar del día actual, creé también "Resultados de ayer".

Hay cosas por mejorar, pero le dediqué más tiempo del que tenía pensado y por ahora lo dejo así. Lo importante es que funciona: ya no me pierdo ningún partido. Los Shortcuts los subo igual, aunque sé que al ser una app de Apple la cantidad de personas que lo pueden usar es limitado.

[Partidos de hoy](https://www.icloud.com/shortcuts/5c011aad34cd45e58e96fee8470c047d)

[Resultados de ayer](https://www.icloud.com/shortcuts/8554581d760d47f2b5cb6dfe5954fa55)