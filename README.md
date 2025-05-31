# InspectorGeoBot: Bot de Telegram para la Consulta Automatizada de Información Catastral (Versión Inicial)

## Descripción General
InspectorGeoBot es un bot de Telegram, actualmente en su **versión inicial de desarrollo (v1.0 - Prototipo)**, concebido para automatizar y agilizar la obtención de información catastral/parcelaria desde un geoportal web específico. Esta primera versión sirve como prueba de concepto funcional y como base para un sistema más completo, con el objetivo principal de reducir drásticamente el tiempo empleado en consultas manuales y minimizar los errores asociados al ingreso de datos para la confección de documentos oficiales (ej. actas).

## El Problema
En muchos organismos, la consulta de datos parcelarios para la elaboración de informes, actas u otros documentos es un proceso manual, repetitivo y propenso a errores. Esto implica:
* Navegación manual a través de portales web complejos.
* Búsqueda e ingreso de coordenadas o identificadores.
* Copia manual de datos relevantes (partida, titular, etc.).
* Pérdida de tiempo productivo y riesgo de inconsistencias en la información.

## La Solución: InspectorGeoBot (v1.0)
La versión actual de InspectorGeoBot ofrece una interfaz conversacional a través de Telegram para realizar estas consultas de forma automática. El usuario simplemente envía una ubicación (coordenadas geográficas o Código Plus) y el bot se encarga de:
1.  Convertir Códigos Plus a coordenadas geográficas (si es necesario, usando la API de Google Geocoding).
2.  Interactuar con el geoportal web designado, simulando la navegación humana mediante técnicas de automatización web (web scraping).
3.  Extraer la información catastral relevante (ej. número de partida, titular del inmueble).
4.  Devolver la información estructurada al usuario directamente en el chat de Telegram, incluyendo una captura de pantalla del terreno marcado en el mapa como evidencia visual para su inclusión en la documentación.

## Características Principales (v1.0)
* Recepción de consultas vía coordenadas (latitud, longitud) o Códigos Plus de Google.
* Integración con la API de Google Geocoding para la resolución de Códigos Plus.
* Automatización de la interacción con geoportales web mediante Selenium.
* Extracción de datos específicos (partida, titular).
* Envío de resultados y capturas de pantalla al usuario a través de Telegram.
* Manejo asíncrono para una experiencia de usuario fluida en Telegram.

## Tecnologías Utilizadas
* **Lenguaje de Programación:** Python
* **Bot Framework:** `python-telegram-bot`
* **Automatización Web/Scraping:** Selenium, WebDriver Manager
* **Interacción HTTP (APIs):** `requests` (para Google Geocoding API)
* **Programación Asíncrona:** `asyncio`
* **APIs Externas:** Google Geocoding API
* **(Se reemplazará en una versión posterior):** `pyautogui` para interacciones específicas de UI (bajo revisión para futuras versiones con el objetivo de implementar alternativas más robustas).

## Estado Actual del Proyecto y Próximos Pasos
InspectorGeoBot se encuentra en su **primera versión funcional (v1.0 - Prototipo)**. Si bien ya demuestra con éxito la capacidad de automatizar el flujo completo de consulta y extracción de datos del geoportal objetivo, representa una **base sólida sobre la cual se planean activamente futuras mejoras, correcciones de errores detectados y la adición de nuevas funcionalidades**.

Los próximos pasos incluyen, entre otros:
* Refinamiento del código existente para mayor eficiencia y mantenibilidad.
* Mejora en el manejo de errores y excepciones.
* Incorporación de nuevas funcionalidades (ej. búsqueda por otros criterios, historial de consultas, exportación de datos).
* Optimización de las interacciones de web scraping para mayor robustez frente a cambios en el geoportal.

## Potencial e Impacto
Incluso en su estado actual, el bot demuestra un gran potencial. A través de las mejoras y nuevas funcionalidades planificadas, este desarrollo tiene el potencial de:
* **Optimizar significativamente los tiempos** de los procesos administrativos que requieren datos catastrales.
* **Reducir errores** de transcripción y asegurar la consistencia de los datos.
* **Liberar recursos humanos** de tareas repetitivas para que puedan enfocarse en actividades de mayor valor.
* **Expandir su utilidad** mediante la integración con otros sistemas, la adaptación a diferentes geoportales (requiriendo análisis y desarrollo específico por portal) y la incorporación de características avanzadas de análisis o reporte.

---

## Acceso al Código Fuente y Contacto
El código fuente completo y la lógica de interacción específica con el geoportal de esta versión inicial se mantienen actualmente en un **repositorio privado**. Esta decisión se debe a la naturaleza específica de la solución, su potencial de desarrollo comercial/estratégico y la necesidad de proteger la lógica de negocio particular implementada, especialmente mientras se encuentra en etapas tempranas de desarrollo.

Si estás interesado en conocer más sobre el proyecto, su evolución, solicitar una demostración de la versión actual, discutir posibles colaboraciones, oportunidades laborales, o explorar cómo una solución similar podría adaptarse a tus necesidades, por favor, no dudes en contactarme:

* **Email:** `lucasdiaz97@hotmail.com`
* **LinkedIn:** `https://www.linkedin.com/in/lucas-diaz-672343149/`


