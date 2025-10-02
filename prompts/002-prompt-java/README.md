# Prompts JRXet para Proyectos Java 8, Java 21 y Programación Reactiva

Este directorio contiene prompts especializados para agentes de IA enfocados en el desarrollo, documentación y revisión de soluciones Java modernas (Java 8, Java 21, Spring Boot, WebFlux, Project Reactor, etc.). Aquí se documentan los archivos de prompt disponibles, su propósito y recomendaciones de uso.

---

## 📄 1. `prompt axet plugin.md`

### Descripción
Prompt diseñado para agentes que operan en entornos donde existe un mecanismo de memoria persistente jerárquica (por ejemplo, plugins tipo "Banco de Memoria" o sistemas de contexto extendido). El agente debe leer y actualizar archivos `.md` estructurados jerárquicamente, que actúan como única fuente de verdad entre sesiones.

### Características principales
- **Obligatoriedad de lectura jerárquica:** Antes de cualquier acción, el agente debe leer todos los archivos en el orden definido.
- **Estructura de memoria:** Define archivos como `projectBrief.md`, `productContext.md`, `techContext.md`, `systemPatterns.md`, y archivos dinámicos como `activeContext.md` y `progress.md`.
- **Foco en Java moderno y reactivo:** Todos los contenidos, scripts y ejemplos están alineados con Java 8, Java 21 y frameworks como Spring Boot, WebFlux y Project Reactor.
- **Reglas estrictas de verificabilidad y ética:** El agente debe citar fuentes, evitar suposiciones y priorizar la precisión.

### Casos de uso recomendados
- Integración con plugins o herramientas de IA que soportan persistencia de contexto mediante archivos.
- Proyectos donde la trazabilidad y la continuidad entre sesiones es crítica.
- Equipos que requieren documentación estructurada y auditable de todo el ciclo de vida del desarrollo Java/Reactivo.

### Limitaciones
- No es adecuado para herramientas de IA que no soportan persistencia de archivos o memoria jerárquica.
- Requiere disciplina en la actualización y consulta de los archivos de memoria.

---

## 📄 2. `prompt general.md`

### Descripción
Prompt universal para agentes de IA expertos en Java 8, Java 21 y programación reactiva, sin dependencia de mecanismos de memoria persistente. Puede ser utilizado en cualquier plataforma de IA (chatbots, asistentes, LLMs) que requiera soporte avanzado para proyectos Java modernos.

### Características principales
- **Independiente de memoria persistente:** No requiere ni asume la existencia de archivos de contexto.
- **Cobertura integral:** Incluye objetivos, entregables, estructura de documentación, consideraciones técnicas y reglas de verificabilidad.
- **Ética y precisión:** Exige citar fuentes, evitar suposiciones y mantener objetividad en todo momento.
- **Compatibilidad:** Puede ser adaptado a cualquier flujo de trabajo, herramienta o plataforma de IA.

### Casos de uso recomendados
- Asistentes conversacionales, chatbots o LLMs sin acceso a archivos persistentes.
- Consultoría, revisión o generación de documentación técnica sobre Java moderno y frameworks reactivos.
- Soporte a equipos de desarrollo que requieren respuestas precisas, verificables y alineadas con las mejores prácticas de Java y frameworks modernos.

### Limitaciones
- No mantiene estado ni continuidad entre sesiones.
- La trazabilidad depende de la plataforma donde se utilice.

---

## 🔑 Diferencias clave

| Prompt                   | ¿Requiere memoria persistente? | ¿Estructura jerárquica de archivos? | ¿Uso recomendado?                        |
|--------------------------|:------------------------------:|:------------------------------------:|------------------------------------------|
| prompt axet plugin.md    | Sí                             | Sí                                   | Plugins, agentes con memoria de archivos |
| prompt general.md        | No                             | No                                   | Cualquier IA, chatbots, LLMs             |

---

## 🛠️ Buenas prácticas de uso

- Selecciona el prompt adecuado según las capacidades de la herramienta de IA.
- En ambos casos, prioriza la precisión, la citación de fuentes y la alineación con la documentación oficial de Java ([Oracle Java Documentation](https://docs.oracle.com/en/java/)), [Spring WebFlux Reference](https://docs.spring.io/spring-framework/docs/current/reference/html/web-reactive.html), [Project Reactor Reference](https://projectreactor.io/docs/core/release/reference/)).
- Si detectas inconsistencias o riesgos técnicos, documenta y sugiere correcciones.
- Mantén la documentación clara, estructurada y fácilmente verificable.

---

## 📌 Notas finales

Estos prompts están diseñados para maximizar la utilidad, trazabilidad y rigor profesional en proyectos Java modernos y reactivos. Adáptalos según las necesidades de tu equipo o plataforma, y consulta siempre la documentación oficial de Java y frameworks relevantes para resolver dudas técnicas complejas.
