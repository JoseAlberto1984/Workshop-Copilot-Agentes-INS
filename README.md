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

...

# 5. Caso Práctico

...

# 6. Buenas Prácticas y Uso Empresarial

...

# 7. Conclusiones

...
