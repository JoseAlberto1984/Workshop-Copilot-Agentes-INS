# 🏛️ Workshop-Copilot-Agentes-INS
Workshop práctico sobre GitHub Copilot, Agentes, Instructions y Skills aplicado al desarrollo moderno con IA.

🏛 Workshop GitHub Copilot y Agentes

Desarrollo Asistido por IA

## 📋 Agenda

1. [Configuración de VS Code para Desarrollo Moderno](#1-configuración-de-vs-code-para-desarrollo-moderno)
2. [Introducción a GitHub Copilot](#2-introducción-a-github-copilot)
3. [Prompts Efectivos](#3-prompts-efectivos)
4. [Agentes, Instructions y Skills](#4-agentes-instructions-y-skills)
5. [Caso Práctico](#5-caso-práctico)
6. [Buenas Prácticas y Uso Empresarial](#6-buenas-prácticas-y-uso-empresarial)
7. [Conclusiones](#7-conclusiones)


--------------------------------------------------

🎯 Objetivo

...

--------------------------------------------------

# 1. Configuración de VS Code para Desarrollo Moderno

## 🎯 Objetivo

Al finalizar esta sección el participante será capaz de:

* Configurar Visual Studio Code para trabajar con Inteligencia Artificial.
* Instalar GitHub Copilot y GitHub Copilot Chat.
* Comprender los modos Ask, Edit y Agent.
* Verificar que GitHub Copilot funciona correctamente.

---

## ¿Por qué Visual Studio Code?

Visual Studio Code se ha convertido en uno de los entornos de desarrollo más utilizados debido a:

* Ligero y multiplataforma.
* Amplio ecosistema de extensiones.
* Integración nativa con GitHub.
* Soporte para GitHub Copilot.
* Compatible con múltiples lenguajes de programación.

---

## Instalación de Visual Studio Code

Descargar la versión estable desde el sitio oficial:

```text
https://code.visualstudio.com
```

Instalar utilizando la configuración predeterminada.

---

## Extensiones Recomendadas

Abrir el administrador de extensiones:

```text
Ctrl + Shift + X
```

Instalar las siguientes extensiones:

| Extensión           | Propósito                 |
| ------------------- | ------------------------- |
| GitHub Copilot      | Asistencia basada en IA   |
| GitHub Copilot Chat | Conversación con IA       |
| C# Dev Kit          | Desarrollo .NET           |
| GitLens             | Integración con Git       |
| Markdown All in One | Creación de documentación |

---

## Inicio de Sesión en GitHub Copilot

1. Instalar la extensión GitHub Copilot.
2. Seleccionar **Sign In with GitHub**.
3. Autorizar el acceso desde GitHub.
4. Confirmar que la licencia de GitHub Copilot está activa.

---

## Verificando que Copilot Funciona

Crear un archivo llamado:

```text
Program.cs
```

Escribir el siguiente comentario:

```csharp
// Crear una clase Cliente para una aseguradora
```

Si Copilot está funcionando correctamente, aparecerá una sugerencia en color gris.

Aceptar la sugerencia utilizando:

```text
TAB
```

---

## Modos de GitHub Copilot

GitHub Copilot dispone de diferentes modos de interacción según la tarea que se desea realizar.

### Modo Ask

Permite realizar consultas y obtener explicaciones.

Ejemplo:

```text
¿Qué es Clean Architecture?
```

Características:

* No modifica archivos.
* Responde preguntas.
* Ideal para aprendizaje y exploración.

---

### Modo Edit

Permite modificar código existente mediante instrucciones en lenguaje natural.

Ejemplo:

```text
Refactoriza este método aplicando principios SOLID.
```

Características:

* Sugiere cambios.
* Solicita aprobación antes de aplicar modificaciones.
* Trabaja sobre archivos existentes.

---

### Modo Agent

Permite ejecutar tareas más completas sobre el proyecto.

Ejemplo:

```text
Crea una API REST para administrar pólizas.
```

Características:

* Analiza el contexto del proyecto.
* Puede crear y modificar múltiples archivos.
* Ayuda a implementar funcionalidades completas.

---

## Ejercicio Práctico

Abrir GitHub Copilot Chat y realizar las siguientes consultas:

### Ejercicio 1

```text
¿Qué es una API REST?
```

### Ejercicio 2

```text
Explícame la diferencia entre .NET Framework y .NET 8.
```

### Ejercicio 3

```text
Genera una clase Cliente para una aseguradora.
```

---

## Resultado Esperado

Al finalizar esta sección el participante debe contar con:

✅ Visual Studio Code instalado

✅ GitHub Copilot configurado

✅ GitHub Copilot Chat habilitado

✅ Primera interacción exitosa con IA

✅ Comprensión básica de los modos Ask, Edit y Agent


# 2. Introducción a GitHub Copilot

## 🎯 Objetivo

Comprender cómo GitHub Copilot puede asistir a los desarrolladores durante el ciclo completo de desarrollo de software, desde la generación de código hasta la documentación y pruebas.

---

## ¿Qué es GitHub Copilot?

GitHub Copilot es un asistente de Inteligencia Artificial integrado en el entorno de desarrollo que ayuda a los desarrolladores mediante sugerencias contextuales y conversaciones en lenguaje natural.

Permite acelerar tareas como:

* Generación de código.
* Explicación de código existente.
* Refactorización.
* Generación de pruebas unitarias.
* Creación de documentación.
* Resolución de errores.
* Generación de consultas SQL.
* Creación de scripts y automatizaciones.

---

## ¿Cómo funciona?

GitHub Copilot analiza:

* El archivo actual.
* El proyecto abierto.
* El contexto de la conversación.
* Los archivos seleccionados.

Y genera respuestas adaptadas al contexto del desarrollo.

```text
Desarrollador
      │
      ▼
 GitHub Copilot
      │
      ▼
 Sugerencias y Respuestas
```

---

## Principales Capacidades

### Generación de Código

A partir de comentarios o instrucciones en lenguaje natural.

Ejemplo:

```csharp
// Crear una clase Cliente para una aseguradora
```

Copilot generará automáticamente una propuesta de implementación.

---

### Explicación de Código

Permite comprender código existente de forma rápida.

Ejemplo:

```text
Explícame este método línea por línea.
```

Ideal para:

* Onboarding de nuevos desarrolladores.
* Comprensión de sistemas heredados.
* Revisión de código.

---

### Refactorización

Permite mejorar código existente.

Ejemplo:

```text
Refactoriza este método aplicando principios SOLID.
```

Copilot sugerirá mejoras en:

* Legibilidad.
* Mantenibilidad.
* Buenas prácticas.

---

### Generación de Pruebas Unitarias

Ejemplo:

```text
Genera pruebas unitarias utilizando XUnit.
```

Puede generar:

* Casos positivos.
* Casos negativos.
* Validaciones.
* Escenarios de error.

---

### Generación de Documentación

Ejemplo:

```text
Genera documentación XML para esta clase.
```

o

```text
Documenta este endpoint REST.
```

---

## Uso del Contexto

Una de las principales fortalezas de GitHub Copilot es su capacidad para utilizar el contexto del proyecto.

### @workspace

Permite consultar información sobre todo el proyecto.

Ejemplos:

```text
@workspace ¿Qué hace este proyecto?
```

```text
@workspace ¿Cómo se implementan los endpoints?
```

```text
@workspace ¿Dónde se define la autenticación?
```

---

### #file

Permite referenciar un archivo específico.

Ejemplo:

```text
Explica el contenido de #file:Program.cs
```

---

### #selection

Permite trabajar únicamente sobre el código seleccionado.

Ejemplo:

```text
Refactoriza #selection aplicando Clean Code.
```

---

## Demostración Práctica

Realizar las siguientes consultas en GitHub Copilot Chat:

### Ejercicio 1

```text
¿Qué es una API REST?
```

### Ejercicio 2

```text
Genera una clase Poliza para una aseguradora.
```

### Ejercicio 3

```text
Genera pruebas unitarias para la clase Poliza.
```

### Ejercicio 4

```text
Documenta la clase utilizando comentarios XML.
```

---

## Beneficios para el Desarrollo

✅ Reduce tareas repetitivas.

✅ Facilita el aprendizaje de nuevas tecnologías.

✅ Acelera la generación de código.

✅ Mejora la calidad mediante sugerencias de buenas prácticas.

✅ Ayuda en la documentación y pruebas.

✅ Incrementa la productividad del equipo.

---

## Consideraciones Importantes

GitHub Copilot es un asistente, no un reemplazo del desarrollador.

Siempre se recomienda:

* Revisar el código generado.
* Validar reglas de negocio.
* Aplicar revisiones de seguridad.
* Ejecutar pruebas antes de desplegar.

---

## Resultado Esperado

Al finalizar esta sección el participante comprenderá:

✅ Qué es GitHub Copilot.

✅ Cómo utilizar Copilot Chat.

✅ Cómo aprovechar el contexto mediante @workspace.

✅ Cómo generar código, pruebas y documentación.

✅ Cuáles son los beneficios y limitaciones de la herramienta.

# 3. Prompts Efectivos

## 🎯 Objetivo

Aprender a redactar instrucciones efectivas para obtener mejores resultados de GitHub Copilot y maximizar el valor de la Inteligencia Artificial durante el desarrollo de software.

---

## ¿Qué es un Prompt?

Un prompt es la instrucción o solicitud que se proporciona a GitHub Copilot para realizar una tarea.

La calidad del resultado depende en gran medida de la calidad del prompt.

```text
Mejor Prompt
      ↓
Mejor Contexto
      ↓
Mejor Resultado
```

---

## Prompt Poco Efectivo

Ejemplo:

```text
Haz una API.
```

Problemas:

* No indica tecnología.
* No define arquitectura.
* No especifica requerimientos.
* No establece restricciones.

El resultado será ambiguo y posiblemente incompleto.

---

## Prompt Más Específico

Ejemplo:

```text
Crea una API REST en .NET 8 para administrar pólizas de seguros.
```

Ahora GitHub Copilot conoce:

* Tecnología.
* Tipo de solución.
* Dominio del negocio.

La calidad de la respuesta mejora considerablemente.

---

## Prompt Bien Estructurado

Ejemplo:

```text
Actúa como Arquitecto de Software.

Diseña una API REST en .NET 8 para administrar pólizas de seguros.

Requisitos:
- Utilizar Minimal API.
- Aplicar Clean Architecture.
- Incluir validaciones.
- Generar pruebas unitarias con XUnit.
- Documentar los endpoints.
```

Este tipo de prompt proporciona:

* Rol.
* Objetivo.
* Restricciones.
* Resultado esperado.

---

## Componentes de un Buen Prompt

### 1. Rol

Indicar el papel que debe asumir la IA.

Ejemplos:

```text
Actúa como Arquitecto de Software.
```

```text
Actúa como Desarrollador Senior .NET.
```

```text
Actúa como Especialista en Seguridad.
```

---

### 2. Objetivo

Definir claramente qué se desea obtener.

Ejemplo:

```text
Diseña una API REST para administrar pólizas.
```

---

### 3. Contexto

Brindar información adicional relevante.

Ejemplo:

```text
La aplicación será utilizada por agentes de seguros.
```

---

### 4. Restricciones

Indicar límites o estándares.

Ejemplo:

```text
Utiliza .NET 8.
No utilices Entity Framework.
Genera comentarios en español.
```

---

### 5. Resultado Esperado

Definir claramente la salida deseada.

Ejemplo:

```text
Genera:
- Entidades
- Endpoints
- Validaciones
- Pruebas unitarias
```

---

## Plantilla Recomendada

```text
Actúa como [ROL].

Objetivo:
[OBJETIVO]

Contexto:
[CONTEXTO]

Restricciones:
[RESTRICCIONES]

Resultado esperado:
[SALIDA DESEADA]
```

---

## Ejemplo Real

### Prompt Básico

```text
Crea una clase Cliente.
```

---

### Prompt Mejorado

```text
Actúa como Desarrollador Senior .NET.

Crea una clase Cliente para una aseguradora.

Requisitos:
- Utilizar C# .NET 8.
- Incluir validaciones básicas.
- Agregar comentarios XML.
- Seguir buenas prácticas de Clean Code.
```

---

## Ejercicio Práctico

### Ejercicio 1

Solicitar a Copilot:

```text
Haz una API.
```

Analizar la respuesta obtenida.

---

### Ejercicio 2

Solicitar:

```text
Crea una API REST en .NET 8 para administrar pólizas de seguros.
```

Comparar los resultados.

---

### Ejercicio 3

Solicitar:

```text
Actúa como Arquitecto de Software.

Diseña una API REST para administrar pólizas.

Requisitos:
- .NET 8
- Minimal API
- XUnit
- Clean Architecture
- Comentarios en español

Genera entidades, endpoints y pruebas unitarias.
```

Comparar nuevamente los resultados.

---

## Buenas Prácticas

✅ Proporcionar contexto.

✅ Definir claramente el objetivo.

✅ Especificar tecnologías.

✅ Indicar restricciones.

✅ Solicitar ejemplos cuando sea necesario.

✅ Dividir problemas complejos en tareas pequeñas.

---

## Errores Comunes

❌ Prompts demasiado generales.

❌ Falta de contexto.

❌ No especificar tecnologías.

❌ Esperar que la IA adivine requerimientos.

❌ Aceptar respuestas sin validarlas.

---

## Resultado Esperado

Al finalizar esta sección el participante será capaz de:

✅ Crear prompts más efectivos.

✅ Obtener respuestas más precisas.

✅ Reducir iteraciones innecesarias.

✅ Aprovechar mejor GitHub Copilot durante el desarrollo.

# 4. Agentes, Instructions y Skills

## 🎯 Objetivo

Comprender cómo los Agentes, Instructions y Skills permiten personalizar y especializar el comportamiento de GitHub Copilot para diferentes escenarios de trabajo.

---

## Evolución del Uso de la IA

La mayoría de los usuarios comienza utilizando GitHub Copilot mediante consultas aisladas:

```text
¿Qué es una API REST?
```

```text
Genera una clase Cliente.
```

```text
Explícame este método.
```

Sin embargo, cuando las tareas se vuelven más complejas, es necesario proporcionar contexto, reglas y comportamiento especializado.

Es aquí donde aparecen los Agentes.

---

## ¿Qué es un Agente?

Un Agente es una configuración especializada que permite a GitHub Copilot actuar bajo un conjunto de reglas, instrucciones y capacidades específicas.

Puede verse como un miembro virtual del equipo con un rol determinado.

Ejemplos:

* Arquitecto de Software
* Desarrollador Backend
* Especialista en Seguridad
* Analista de Negocio
* Revisor de Código
* Especialista en Pruebas

---

## Diferencia entre Chat y Agente

### Chat Tradicional

Cada conversación inicia prácticamente desde cero.

```text
Usuario
   │
   ▼
GitHub Copilot
```

---

### Agente

El agente incorpora conocimiento, reglas y comportamiento especializado.

```text
Usuario
   │
   ▼
Agente
   │
   ├── Instructions
   ├── Skills
   │
   ▼
GitHub Copilot
```

---

## Beneficios de Utilizar Agentes

✅ Respuestas más consistentes.

✅ Menor necesidad de repetir instrucciones.

✅ Aplicación automática de estándares.

✅ Mejor alineación con las prácticas del equipo.

✅ Mayor productividad.

---

## ¿Qué son las Instructions?

Las Instructions son reglas permanentes que definen cómo debe comportarse el agente.

Permiten establecer:

* Idioma de respuesta.
* Estilo de desarrollo.
* Arquitectura recomendada.
* Convenciones del equipo.
* Restricciones técnicas.

---

### Ejemplo de Instructions

```text
Eres un Arquitecto de Software.

Debes responder en español.

Debes utilizar .NET 8.

Debes promover Clean Architecture.

Debes sugerir pruebas unitarias cuando sea posible.

Debes seguir buenas prácticas de seguridad.
```

---

## Beneficios de las Instructions

Sin Instructions:

```text
Genera una API.
```

El resultado puede variar entre conversaciones.

---

Con Instructions:

```text
Genera una API.
```

El agente responderá aplicando automáticamente:

* .NET 8
* Clean Architecture
* Buenas prácticas
* Pruebas unitarias

---

## ¿Qué son los Skills?

Los Skills representan capacidades o conocimientos especializados que un agente puede utilizar para resolver tareas.

Un Skill puede ayudar al agente a:

* Generar código.
* Analizar proyectos.
* Crear documentación.
* Diseñar arquitecturas.
* Revisar calidad de código.
* Generar pruebas.

---

## Ejemplo Conceptual

### Agente Arquitecto

Instructions:

```text
Responde como Arquitecto de Software.
```

Skills:

```text
Diseño de APIs
Diseño de Arquitectura
Buenas Prácticas
Patrones de Diseño
```

---

### Agente QA

Instructions:

```text
Responde como Especialista QA.
```

Skills:

```text
Pruebas Unitarias
Pruebas de Integración
Cobertura de Código
Automatización
```

---

## Caso de Uso

Supongamos que un desarrollador solicita:

```text
Necesito una API para administrar pólizas.
```

Un agente configurado como Arquitecto podría responder:

* Arquitectura propuesta.
* Capas recomendadas.
* Entidades principales.
* Endpoints sugeridos.
* Estrategia de pruebas.
* Consideraciones de seguridad.

Todo esto sin necesidad de indicar cada detalle manualmente.

---

## Cuándo Utilizar un Agente

Se recomienda utilizar agentes cuando:

* Existen estándares definidos.
* Se trabaja en equipos grandes.
* Se desea consistencia en las respuestas.
* Se realizan tareas repetitivas.
* Se busca acelerar la incorporación de nuevos colaboradores.

---

## Ejercicio Práctico

Imagine que debe crear un agente para su equipo.

Defina:

### Rol

```text
Arquitecto de Software
```

### Instructions

```text
Responde en español.

Utiliza .NET 8.

Aplica Clean Architecture.

Sugiere pruebas unitarias.
```

### Skills

```text
Diseño de APIs
Arquitectura de Software
Buenas Prácticas
Pruebas Unitarias
```

Analice cómo estas configuraciones podrían influir en las respuestas generadas por GitHub Copilot.

---

## Resultado Esperado

Al finalizar esta sección el participante comprenderá:

✅ Qué es un Agente.

✅ Qué son las Instructions.

✅ Qué son los Skills.

✅ Cómo los agentes permiten especializar GitHub Copilot.

✅ Cuándo resulta conveniente utilizar agentes en entornos empresariales.

# 5. Caso Práctico

## 🎯 Objetivo

Demostrar cómo un Agente especializado puede ayudar a resolver una necesidad real de desarrollo de software aplicando automáticamente buenas prácticas, lineamientos y estándares definidos por el equipo.

---

## Escenario

Un equipo de desarrollo necesita construir una nueva API para administrar pólizas de seguros.

La organización ha definido los siguientes estándares:

* Desarrollo en .NET 8.
* Uso de Clean Architecture.
* Implementación de pruebas unitarias.
* Documentación de endpoints.
* Aplicación de buenas prácticas de seguridad.

El objetivo es evitar que cada desarrollador tenga que recordar y especificar estos requisitos manualmente en cada consulta.

---

## Solución Tradicional

Un desarrollador podría realizar una consulta como:

```text
Genera una API para administrar pólizas.
```

Sin embargo, el resultado dependerá completamente del contexto disponible y podría no seguir los estándares definidos por la organización.

---

## Solución Utilizando un Agente

Se crea un agente especializado llamado:

```text
Arquitecto de Software
```

---

## Instructions del Agente

```text
Eres un Arquitecto de Software.

Debes responder en español.

Debes utilizar .NET 8.

Debes promover Clean Architecture.

Debes sugerir pruebas unitarias.

Debes aplicar buenas prácticas de seguridad.

Debes generar soluciones mantenibles y escalables.
```

---

## Skills del Agente

```text
Diseño de APIs

Arquitectura de Software

Patrones de Diseño

Buenas Prácticas

Pruebas Unitarias

Documentación Técnica
```

---

## Consulta Realizada

```text
Necesito una API para administrar pólizas de seguros.
```

---

## Resultado Esperado

El agente podría responder proponiendo:

### Arquitectura

```text
API

Aplicación

Dominio

Infraestructura
```

---

### Entidades

```text
Poliza

Cliente

Cobertura
```

---

### Endpoints

```http
GET     /api/polizas

GET     /api/polizas/{id}

POST    /api/polizas

PUT     /api/polizas/{id}

DELETE  /api/polizas/{id}
```

---

### Pruebas

```text
Pruebas Unitarias

Pruebas de Integración

Validaciones de Negocio
```

---

### Seguridad

```text
Autenticación

Autorización

Validación de Entradas

Manejo de Errores
```

---

## Beneficios Obtenidos

Sin agente:

* Cada desarrollador realiza consultas diferentes.
* Resultados inconsistentes.
* Mayor riesgo de incumplir estándares.

Con agente:

* Respuestas alineadas con la organización.
* Menor esfuerzo de configuración.
* Mayor consistencia.
* Mejor calidad técnica.

---

## Discusión

Analice con el grupo:

### ¿Qué otras especializaciones podrían implementarse?

Ejemplos:

* Agente QA.
* Agente DevOps.
* Agente Seguridad.
* Agente Analista de Negocio.
* Agente Documentador.

---

## Resultado Esperado

Al finalizar este ejercicio el participante comprenderá:

✅ Cómo un agente puede especializar el comportamiento de GitHub Copilot.

✅ Cómo las Instructions influyen en las respuestas.

✅ Cómo los Skills aportan capacidades especializadas.

✅ Cómo los agentes ayudan a estandarizar el desarrollo dentro de una organización.

# 6. Buenas Prácticas y Uso Empresarial

## 🎯 Objetivo

Conocer las principales recomendaciones para utilizar GitHub Copilot de forma segura, responsable y efectiva dentro de entornos empresariales.

---

## GitHub Copilot como Asistente

Es importante comprender que GitHub Copilot es un asistente para el desarrollo de software.

Su propósito es ayudar a los desarrolladores a:

* Generar código.
* Resolver dudas técnicas.
* Crear documentación.
* Generar pruebas.
* Acelerar tareas repetitivas.

Sin embargo, las decisiones finales continúan siendo responsabilidad del equipo de desarrollo.

---

## Principio Fundamental

> GitHub Copilot asiste al desarrollador, pero no reemplaza su criterio técnico.

Todo código generado debe ser revisado antes de ser incorporado a una solución.

---

## Seguridad de la Información

Antes de utilizar GitHub Copilot, es importante considerar las políticas de seguridad de la organización.

### Evitar compartir información sensible

No se recomienda incluir:

* Contraseñas.
* Tokens de acceso.
* Secretos de aplicaciones.
* Llaves criptográficas.
* Información confidencial de clientes.
* Datos personales sensibles.

Ejemplos:

❌ Incorrecto

```text id="1f8zvj"
Mi contraseña de producción es...
```

```text id="tt57pp"
Este es el token de acceso del sistema...
```

---

### Buenas Prácticas

✅ Utilizar datos ficticios para ejemplos.

✅ Ocultar información sensible.

✅ Revisar las políticas internas de la organización.

---

## Validación del Código Generado

Aunque GitHub Copilot genera código funcional, siempre se recomienda validar:

* Correctitud funcional.
* Seguridad.
* Rendimiento.
* Cumplimiento de estándares internos.

---

### Revisar Siempre

Antes de aceptar código generado:

* Comprender la solución propuesta.
* Verificar dependencias.
* Revisar excepciones y validaciones.
* Confirmar cumplimiento de reglas de negocio.

---

## Uso Responsable de la Inteligencia Artificial

La IA puede acelerar el trabajo, pero no debe sustituir:

* Análisis técnico.
* Diseño de arquitectura.
* Revisión de código.
* Validación funcional.
* Pruebas.

---

## Uso de Prompts Claros

Prompts bien estructurados generan mejores resultados.

Ejemplo:

❌ Poco claro

```text id="t6dz6h"
Haz una API.
```

---

✅ Más efectivo

```text id="4t9vx9"
Crea una API REST en .NET 8 para administrar pólizas utilizando Clean Architecture.
```

---

## Mantener Consistencia

Cuando se trabaja en equipo es recomendable:

* Definir estándares.
* Compartir instrucciones comunes.
* Utilizar agentes especializados.
* Documentar lineamientos.

Esto ayuda a obtener resultados más consistentes entre diferentes desarrolladores.

---

## Revisión de Código

El código generado por GitHub Copilot debe seguir el mismo proceso de revisión que cualquier otro desarrollo.

Se recomienda:

* Pull Requests.
* Code Reviews.
* Pruebas automatizadas.
* Validaciones de seguridad.

---

## Medición del Valor

GitHub Copilot debe considerarse una herramienta de productividad.

Algunas métricas que pueden analizarse son:

* Tiempo de desarrollo.
* Reducción de tareas repetitivas.
* Velocidad de generación de pruebas.
* Velocidad de documentación.
* Productividad del equipo.

---

## Casos de Uso Recomendados

GitHub Copilot suele aportar mayor valor en:

### Desarrollo

* Generación de código.
* Refactorización.
* Creación de APIs.
* Consultas SQL.

### Calidad

* Pruebas unitarias.
* Pruebas de integración.
* Casos de prueba.

### Documentación

* Comentarios XML.
* Documentación técnica.
* Diagramas y descripciones.

### Aprendizaje

* Nuevos lenguajes.
* Nuevos frameworks.
* Patrones de diseño.
* Buenas prácticas.

---

## Casos donde se debe tener mayor cuidado

Se recomienda una revisión más rigurosa cuando el código involucra:

* Seguridad.
* Autenticación.
* Autorización.
* Criptografía.
* Procesamiento financiero.
* Datos sensibles.
* Integraciones críticas.

---

## Recomendaciones para Equipos

### Hacer

✅ Utilizar GitHub Copilot como apoyo.

✅ Validar el código generado.

✅ Aplicar revisiones de código.

✅ Compartir buenas prácticas.

✅ Utilizar prompts claros.

✅ Definir estándares comunes.

---

### Evitar

❌ Confiar ciegamente en las respuestas.

❌ Compartir información sensible.

❌ Omitir pruebas.

❌ Omitir revisiones de seguridad.

❌ Incorporar código sin comprenderlo.

---

## Resultado Esperado

Al finalizar esta sección el participante comprenderá:

✅ Cómo utilizar GitHub Copilot de forma responsable.

✅ Qué información no debe compartirse.

✅ La importancia de validar el código generado.

✅ Cómo integrar GitHub Copilot dentro de los procesos de desarrollo existentes.

✅ Buenas prácticas para el uso empresarial de la Inteligencia Artificial.

# 7. Conclusiones

## 🎯 Objetivo

Recapitular los principales conceptos vistos durante el taller y establecer una ruta de adopción para comenzar a utilizar GitHub Copilot de forma efectiva en el trabajo diario.

---

## ¿Qué Aprendimos?

Durante este taller se abordaron los principales conceptos para iniciar en el desarrollo asistido por Inteligencia Artificial utilizando GitHub Copilot.

### Configuración del Entorno

Se configuró Visual Studio Code para trabajar con herramientas de Inteligencia Artificial.

Se instalaron y configuraron:

* GitHub Copilot.
* GitHub Copilot Chat.
* Extensiones complementarias para desarrollo moderno.

---

### Uso de GitHub Copilot

Se exploraron capacidades como:

* Generación de código.
* Explicación de código existente.
* Refactorización.
* Generación de pruebas unitarias.
* Documentación técnica.

---

### Prompts Efectivos

Se comprobó cómo la calidad de los resultados depende directamente de la calidad de las instrucciones proporcionadas.

Se analizaron elementos como:

* Rol.
* Contexto.
* Restricciones.
* Resultado esperado.

---

### Agentes, Instructions y Skills

Se comprendió cómo especializar el comportamiento de GitHub Copilot mediante:

* Agentes.
* Instructions.
* Skills.

Permitiendo respuestas más consistentes y alineadas con los estándares de una organización.

---

### Caso Práctico

Se analizó un escenario real donde un agente especializado puede ayudar a:

* Diseñar soluciones.
* Aplicar buenas prácticas.
* Mantener consistencia técnica.
* Acelerar el desarrollo.

---

### Buenas Prácticas

Se revisaron aspectos relacionados con:

* Seguridad.
* Calidad.
* Gobierno.
* Uso responsable de la Inteligencia Artificial.

---

## Principales Mensajes

### GitHub Copilot es un Asistente

GitHub Copilot ayuda a acelerar el trabajo del desarrollador, pero no reemplaza el análisis técnico, la experiencia ni la responsabilidad profesional.

---

### La Calidad del Resultado Depende del Contexto

Mientras mejor sea el prompt, mejor será el resultado.

La IA necesita contexto para generar respuestas más precisas y útiles.

---

### Los Agentes Permiten Escalar el Uso de la IA

Los agentes ayudan a incorporar:

* Estándares.
* Buenas prácticas.
* Conocimiento organizacional.
* Consistencia entre equipos.

---

### La IA Debe Integrarse al Proceso de Desarrollo

El uso de Inteligencia Artificial debe complementar prácticas existentes como:

* Revisión de código.
* Pruebas unitarias.
* Pruebas de integración.
* Seguridad.
* Gobierno de software.

---

## ¿Qué Puedo Hacer Mañana?

Al finalizar este taller se recomienda comenzar con pequeñas acciones:

### Nivel 1

Utilizar GitHub Copilot para:

* Generar código repetitivo.
* Crear pruebas unitarias.
* Generar documentación.

---

### Nivel 2

Utilizar prompts más estructurados.

Incorporar:

* Rol.
* Contexto.
* Restricciones.
* Resultado esperado.

---

### Nivel 3

Crear agentes especializados para diferentes necesidades:

* Arquitectura.
* Desarrollo.
* Calidad.
* Seguridad.
* Documentación.

---

## Próximos Pasos

Una vez dominados estos conceptos, es posible avanzar hacia escenarios más avanzados:

* Agentes empresariales.
* Automatización de procesos.
* Integración con herramientas corporativas.
* Inteligencia Artificial aplicada al ciclo completo de desarrollo.

---

## Reflexión Final

> La Inteligencia Artificial no reemplaza a los desarrolladores; potencia sus capacidades.

Las organizaciones que logren combinar la experiencia de sus equipos con el uso adecuado de herramientas como GitHub Copilot estarán mejor preparadas para desarrollar soluciones de mayor calidad, en menor tiempo y con mayor capacidad de adaptación a los cambios del negocio.

---

## ¡Gracias por Participar!

### Preguntas y Respuestas

Espacio abierto para consultas, comentarios y experiencias relacionadas con el uso de GitHub Copilot y Agentes.


