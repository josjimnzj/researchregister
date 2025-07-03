# Plataforma de Encuestas Inteligente para Ejecutivos

Una aplicación web SPA diseñada para optimizar el proceso de entrevistas. Permite a los ejecutivos guiar a los entrevistados a través de un formulario dinámico, capturar respuestas de manera estructurada y obtener análisis instantáneos generados por IA, como resúmenes ejecutivos y planes de acción, directamente desde la interfaz.

---

## ✨ Características Principales

### 1. **Interfaz de Doble Panel**
El diseño se divide en dos secciones principales para una máxima eficiencia:
- **Panel de Preguntas (Izquierda):** Un área amplia y limpia donde se presentan las preguntas una por una, manteniendo el enfoque del usuario.
- **Panel de Progreso (Derecha):** Un historial en tiempo real que muestra todas las preguntas respondidas, permitiendo una revisión rápida del progreso de la encuesta.

### 2. **Flujo de Preguntas Dinámico**
La encuesta no es lineal. Utiliza lógica condicional en JavaScript para adaptar las preguntas siguientes basándose en las respuestas anteriores. Por ejemplo, solo pregunta sobre el tipo de mascota si el usuario ha confirmado que tiene una.

### 3. **Navegación e Historial Inteligente**
- **Navegación Paso a Paso:** Botones claros de "Siguiente" y "Anterior" para un movimiento secuencial.
- **Edición Rápida:** El panel de progreso permite al ejecutivo hacer doble clic o usar un icono de edición en cualquier respuesta anterior para saltar directamente a esa pregunta y modificarla. El flujo de respuestas subsiguientes se borra automáticamente para mantener la coherencia de los datos.
- **Bloqueo de Historial:** Una vez que la encuesta se graba para su análisis, el panel de progreso se bloquea visual y funcionalmente, impidiendo modificaciones post-análisis y garantizando la integridad de los datos.

### 4. **Análisis Automatizado con IA (API de Gemini)**
Al finalizar la recolección de datos, el ejecutivo puede "Grabar y Analizar" las respuestas. Esta acción desencadena dos llamadas a la API de Gemini:
- **Sugerencias de la IA:** Genera automáticamente una lista de próximos pasos o áreas de desarrollo para el entrevistado.
- **Resumen Ejecutivo:** Crea un resumen profesional del perfil del entrevistado, ideal para informes de RR.HH. o gestión.

### 5. **Interfaz de Resultados con Pestañas**
Los resultados del análisis de la IA se presentan en una interfaz de pestañas limpia y moderna:
- La pestaña de "Sugerencias" se muestra por defecto.
- El "Resumen Ejecutivo" se genera bajo demanda cuando se hace clic en su pestaña, optimizando el rendimiento.

### 6. **Diseño Moderno y Responsivo**
- Construido con **Tailwind CSS** para una estética limpia, profesional y totalmente adaptable a dispositivos móviles, tabletas y ordenadores de escritorio.
- Utiliza la fuente **Inter** para una excelente legibilidad.
- Incluye microinteracciones como animaciones de entrada y un modal de carga para una experiencia de usuario fluida.

---

## 🚀 Tecnologías Utilizadas

- **HTML5:** Para la estructura semántica del formulario.
- **Tailwind CSS:** Para todo el diseño y la responsividad.
- **JavaScript (Vanilla):** Para toda la lógica interactiva, manejo del estado, flujo condicional y llamadas a la API.
- **API de Google Gemini:** Para las funcionalidades de inteligencia artificial.

---

## ⚙️ Uso

Este proyecto es un único archivo `index.html` autocontenido. Para utilizarlo, simplemente ábrelo en cualquier navegador web moderno. No requiere un servidor ni pasos de compilación.
