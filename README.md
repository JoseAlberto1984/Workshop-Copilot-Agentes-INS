# 🏛️ Workshop-Copilot-Agentes
Workshop práctico sobre GitHub Copilot, Agentes, Instructions y Skills aplicado al desarrollo moderno con IA.

🏛 Workshop GitHub Copilot y Agentes

Desarrollo Asistido por IA

## 📋 Agenda
``
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
* Comprender los modos Ask, Plan y Agent.
* Verificar que GitHub Copilot funciona correctamente.
* Iniciar el desarrollo de una solución empresarial relacionada con seguros.

---

## Escenario del Taller

Durante todo el workshop se desarrollará una solución llamada:

```text
Workshop.Seguros.API
```

Esta solución representará una API empresarial para la administración de solicitudes relacionadas con seguros.

A lo largo de las diferentes secciones del taller iremos incorporando nuevos conocimientos y funcionalidades, permitiendo observar cómo GitHub Copilot puede asistir durante todo el ciclo de desarrollo de software.

La solución evolucionará progresivamente conforme se introduzcan nuevos conceptos y capacidades.

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

## Creación del Workspace del Taller

Durante todo el workshop trabajaremos sobre un único workspace llamado:

```text
Workshop.Seguros.API
```

Crear una carpeta con el nombre:

```text
Workshop.Seguros.API
```

Abrir la carpeta en Visual Studio Code mediante:

```text
File → Open Folder
```

o utilizando:

```text
Ctrl + K Ctrl + O
```

Esta carpeta representará el workspace del proyecto y será utilizada durante todas las secciones del taller.

---

## Creación de la Solución con GitHub Copilot

En lugar de crear manualmente la solución, utilizaremos GitHub Copilot en modo Agent.

Abrir GitHub Copilot Chat y seleccionar:

```text
Agent
```

Realizar la siguiente solicitud:

```text
Crea una solución .NET 8 llamada Workshop.Seguros.API.

La solución debe contener un proyecto Web API con el mismo nombre.

Genera la estructura básica del proyecto utilizando ASP.NET Core Minimal APIs.

Mantén Swagger habilitado.

No agregues entidades ni lógica de negocio todavía.

Elimina el endpoint WeatherForecast y cualquier clase asociada.

Deja la aplicación lista para comenzar a construir endpoints relacionados con solicitudes de seguro.
```

---

## Primera Interacción con GitHub Copilot

Una vez creada la solución, solicitar:

```text
Crea una carpeta llamada Entidades.

Dentro de ella genera una clase llamada SolicitudSeguro.

Utiliza Guid como identificador único.

La entidad debe incluir:

- Id
- NumeroSolicitud
- IdentificacionCliente
- NombreCliente
- FechaSolicitud
- TipoSeguro
- Estado

Inicializa las colecciones necesarias y utiliza tipos apropiados para una aplicación empresarial.
```

Copilot propondrá la creación de la carpeta y del archivo:

```text
Entidades
└── SolicitudSeguro.cs
```

Aceptar los cambios sugeridos.

---

## Verificando que GitHub Copilot Funciona

Abrir el archivo:

```text
SolicitudSeguro.cs
```

y solicitar:

```text
Explica esta clase línea por línea.
```

Posteriormente solicitar:

```text
Agrega comentarios XML a todas las propiedades.
```

Si GitHub Copilot responde correctamente y propone cambios sobre el archivo, significa que la integración se encuentra funcionando adecuadamente.

---

## Estructura Esperada

Al finalizar esta sección, la solución podría tener una estructura similar a:

```text
Workshop.Seguros.API
│
├── Workshop.Seguros.API.sln
│
├── Workshop.Seguros.API
│   ├── Program.cs
│   ├── appsettings.json
│   └── Entidades
│       └── SolicitudSeguro.cs
│
└── Properties
```

---

## Compilando y Ejecutando la Aplicación

Una vez creada la solución, es recomendable verificar que todo se haya generado correctamente.

### Paso 1

Abrir una terminal en Visual Studio Code mediante:

```text
Terminal → New Terminal
```

o utilizando:

```text
Ctrl + Shift + `
```

---

### Paso 2

Asegurarse de estar ubicado dentro del proyecto Web API.

La carpeta del proyecto debe contener archivos similares a:

```text
Program.cs
appsettings.json
appsettings.Development.json
```

Si es necesario, cambiarse al directorio correspondiente.

Por ejemplo:

```bash
cd Workshop.Seguros.API
```

o al directorio que contenga el archivo:

```text
Program.cs
```

---

### Paso 3

Compilar la aplicación ejecutando:

```bash
dotnet build
```

Verificar que la compilación finalice correctamente y que no existan errores.

---

### Paso 4

Ejecutar la aplicación mediante:

```bash
dotnet run
```

La consola mostrará una salida similar a:

```text
Now listening on: https://localhost:7147
Now listening on: http://localhost:5147
```

---

### Paso 5

Copiar la dirección HTTPS mostrada en la consola y agregar:

```text
/swagger/index.html
```

Por ejemplo:

```text
https://localhost:7147/swagger/index.html
```

---

### Paso 6

Verificar que se despliegue correctamente la interfaz de Swagger.

Si todo se encuentra correcto, se visualizarán los endpoints expuestos por la API y será posible realizar pruebas directamente desde el navegador.

Este será el mecanismo que utilizaremos durante el resto del workshop para validar las funcionalidades desarrolladas.

---

## Verificación de la Aplicación

Al finalizar este ejercicio se habrá comprobado que:

✅ La solución fue creada correctamente.

✅ El proyecto compila sin errores.

✅ La aplicación puede ejecutarse localmente.

✅ Swagger se encuentra habilitado.

✅ Es posible probar los endpoints desde el navegador.

✅ La API está lista para continuar con las siguientes secciones del workshop.


# 2. Introducción a GitHub Copilot

## 🎯 Objetivo

Comprender cómo GitHub Copilot puede asistir a los desarrolladores durante el ciclo completo de desarrollo de software, desde la generación de código hasta la documentación y pruebas.

Durante esta sección continuaremos desarrollando la solución:

```text
Workshop.Seguros.API
```

relacionada con la administración de solicitudes de seguros.

---

# ¿Qué es GitHub Copilot?

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

En este workshop utilizaremos GitHub Copilot para construir progresivamente una solución empresarial relacionada con seguros.

---

# ¿Cómo funciona?

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
      │
      ▼
Proyecto Workshop.Seguros.API
```

---

# Principales Capacidades

## Generación de Código

A partir de comentarios o instrucciones en lenguaje natural.

Ejemplo:

```csharp
// Crear una entidad SolicitudSeguro para una aplicación relacionada con seguros
```

Copilot generará automáticamente una propuesta de implementación.

---

## Explicación de Código

Permite comprender código existente de forma rápida.

Ejemplo:

```text
Explícame esta clase línea por línea.
```

Ideal para:

* Onboarding de nuevos desarrolladores.
* Comprensión de sistemas heredados.
* Revisión de código.
* Aprendizaje de nuevas tecnologías.

---

## Refactorización

Permite mejorar código existente.

Ejemplo:

```text
Refactoriza esta entidad aplicando principios SOLID y Clean Code.
```

Copilot sugerirá mejoras en:

* Legibilidad.
* Mantenibilidad.
* Buenas prácticas.
* Organización del código.

---

## Generación de Pruebas Unitarias

Ejemplo:

```text
Genera pruebas unitarias utilizando XUnit para la entidad SolicitudSeguro.
```

Puede generar:

* Casos positivos.
* Casos negativos.
* Validaciones.
* Escenarios de error.

---

## Generación de Documentación

Ejemplo:

```text
Genera comentarios XML para esta clase.
```

o

```text
Documenta este endpoint REST.
```

---

# Uso del Contexto

Una de las principales fortalezas de GitHub Copilot es su capacidad para utilizar el contexto del proyecto.

---

## @workspace

Permite consultar información sobre toda la solución.

Ejemplos:

```text
@workspace ¿Qué hace este proyecto?
```

```text
@workspace ¿Cuáles son las entidades existentes?
```

```text
@workspace ¿Cómo podría estructurarse esta API utilizando Clean Architecture?
```

```text
@workspace ¿Dónde debería ubicarse la lógica de negocio?
```

---

## #file

Permite trabajar sobre un archivo específico.

Ejemplo:

```text
Explica el contenido de #file:SolicitudSeguro.cs
```

o

```text
Genera comentarios XML para #file:SolicitudSeguro.cs
```

---

## #selection

Permite trabajar únicamente sobre el código seleccionado.

Ejemplo:

```text
Refactoriza #selection aplicando Clean Code.
```

---

# Demostración Práctica

Continuaremos ampliando la solución Workshop.Seguros.API.

---

## Ejercicio 1

Solicitar a GitHub Copilot:

```text
Genera una entidad Cliente para una aplicación relacionada con seguros.

Debe incluir:

- Id
- Identificacion
- NombreCompleto
- FechaNacimiento
- Telefono
- CorreoElectronico
```

---

## Ejercicio 2

Solicitar:

```text
Genera una entidad Cobertura.

Debe incluir:

- Id
- Nombre
- Descripcion
- MontoMaximo
- Activa
```

---

## Ejercicio 3

Solicitar:

```text
Genera una entidad DocumentoAdjunto.

Debe incluir:

- Id
- NombreArchivo
- TipoContenido
- TamanoBytes
- FechaCarga
```

---

## Ejercicio 4

Solicitar:

```text
Genera una relación entre SolicitudSeguro y DocumentoAdjunto.

Una solicitud puede tener múltiples documentos adjuntos.

En la entidad SolicitudSeguro agrega una colección de DocumentoAdjunto.

En la entidad DocumentoAdjunto agrega únicamente la propiedad SolicitudSeguroId para representar la relación.

No agregues una propiedad de navegación SolicitudSeguro dentro de DocumentoAdjunto.

La solución debe poder serializarse y deserializarse correctamente desde Swagger utilizando JSON.
```

---

### Nota

Para simplificar las pruebas del workshop, la entidad `DocumentoAdjunto` solamente tendrá una referencia mediante `SolicitudSeguroId`.

Esto evita relaciones circulares y problemas de serialización o deserialización al probar el endpoint `POST /api/solicitudes-seguro` desde Swagger.

La estructura esperada sería:

```csharp
public class SolicitudSeguro
{
    // Propiedades...

    public List<DocumentoAdjunto> DocumentosAdjuntos { get; set; } = new();
}

public class DocumentoAdjunto
{
    public int Id { get; set; }
    public string NombreArchivo { get; set; } = string.Empty;
    public string TipoContenido { get; set; } = string.Empty;
    public long TamanoBytes { get; set; }
    public DateTime FechaCarga { get; set; }

    public int? SolicitudSeguroId { get; set; }
}
```
---

## Ejercicio 5

Solicitar:

```text
Genera pruebas unitarias utilizando XUnit para la entidad SolicitudSeguro.
```

---

## Ejercicio 6

Solicitar:

```text
Genera comentarios XML para todas las propiedades de la entidad SolicitudSeguro.
```

---

## Ejercicio 7

Solicitar:

```text
Explica la clase SolicitudSeguro línea por línea.
```

---

# Construcción del Primer CRUD

Hasta este momento hemos utilizado GitHub Copilot para generar entidades y comprender mejor la estructura del proyecto.

A continuación, aprovecharemos sus capacidades para construir el primer CRUD de la solución.

Los endpoints que implementaremos serán:

```http
GET     /api/solicitudes-seguro

GET     /api/solicitudes-seguro/{id}

POST    /api/solicitudes-seguro

PUT     /api/solicitudes-seguro/{id}

DELETE  /api/solicitudes-seguro/{id}
```

Este ejercicio permitirá observar cómo GitHub Copilot puede asistir en la implementación de funcionalidades reales de una API.

---

## Ejercicio 8

Solicitar:

```text
Genera un endpoint REST en .NET 8 para obtener todas las solicitudes de seguro.

No agregues código directamente en Program.cs.

Crea una carpeta llamada Endpoints.

Dentro de ella crea el archivo ObtenerSolicitudesSeguro.cs.

Utiliza una clase estática y un método de extensión llamado MapObtenerSolicitudesSeguro.

Program.cs debe permanecer limpio y únicamente invocar los métodos de extensión de los endpoints.

Agrega comentarios XML y utiliza Minimal APIs.
```

Revisar la propuesta generada y aceptar los cambios sugeridos.

---

## Ejercicio 9

Solicitar:

```text
Genera un endpoint REST para obtener una solicitud de seguro por Id.

No agregues código directamente en Program.cs.

Utiliza la carpeta Endpoints.

Crea el archivo ObtenerSolicitudSeguroPorId.cs.

Utiliza una clase estática y un método de extensión llamado MapObtenerSolicitudSeguroPorId.

Utiliza la entidad SolicitudSeguro existente.

Agrega comentarios XML y utiliza Minimal APIs.
```

Aceptar los cambios sugeridos.

---

## Ejercicio 10

Solicitar:

```text
Genera un endpoint REST para registrar una solicitud de seguro.

No agregues código directamente en Program.cs.

Utiliza la carpeta Endpoints.

Crea el archivo CrearSolicitudSeguro.cs.

Utiliza una clase estática y un método de extensión llamado MapCrearSolicitudSeguro.

Utiliza la entidad SolicitudSeguro existente.

Agrega comentarios XML y utiliza Minimal APIs.
```

Aceptar los cambios sugeridos.

---

## Ejercicio 11

Solicitar:

```text
Genera un endpoint REST para actualizar una solicitud de seguro existente.

No agregues código directamente en Program.cs.

Utiliza la carpeta Endpoints.

Crea el archivo ActualizarSolicitudSeguro.cs.

Utiliza una clase estática y un método de extensión llamado MapActualizarSolicitudSeguro.

Utiliza la entidad SolicitudSeguro existente.

Agrega comentarios XML y utiliza Minimal APIs.
```

Aceptar los cambios sugeridos.

---

## Ejercicio 12

Solicitar:

```text
Genera un endpoint REST para eliminar una solicitud de seguro por Id.

No agregues código directamente en Program.cs.

Utiliza la carpeta Endpoints.

Crea el archivo EliminarSolicitudSeguro.cs.

Utiliza una clase estática y un método de extensión llamado MapEliminarSolicitudSeguro.

Utiliza la entidad SolicitudSeguro existente.

Agrega comentarios XML y utiliza Minimal APIs.
```

Aceptar los cambios sugeridos.

---

## Verificando el CRUD con Swagger

Ejecutar nuevamente la aplicación:

```bash
dotnet run
```

Abrir Swagger desde el navegador:

```text
https://localhost:xxxx/swagger/index.html
```

Verificar que se encuentren disponibles los siguientes endpoints:

```http
GET     /api/solicitudes-seguro

GET     /api/solicitudes-seguro/{id}

POST    /api/solicitudes-seguro

PUT     /api/solicitudes-seguro/{id}

DELETE  /api/solicitudes-seguro/{id}
```

---

## Resultado Esperado

Al finalizar este ejercicio, la solución podría tener una estructura similar a:

```text
Workshop.Seguros.API
│
├── Entidades
│   ├── SolicitudSeguro.cs
│   ├── Cliente.cs
│   ├── Cobertura.cs
│   └── DocumentoAdjunto.cs
│
├── Endpoints
│   ├── ObtenerSolicitudesSeguro.cs
│   ├── ObtenerSolicitudSeguroPorId.cs
│   ├── CrearSolicitudSeguro.cs
│   ├── ActualizarSolicitudSeguro.cs
│   └── EliminarSolicitudSeguro.cs
│
├── Program.cs
└── appsettings.json
```

En este punto, la solución ya contará con un CRUD funcional generado con ayuda de GitHub Copilot y validado mediante Swagger.

En las siguientes secciones veremos cómo obtener mejores resultados utilizando prompts más efectivos y cómo extender las capacidades de GitHub Copilot mediante Agentes, Instructions y Skills.


# Beneficios para el Desarrollo

✅ Reduce tareas repetitivas.

✅ Facilita el aprendizaje de nuevas tecnologías.

✅ Acelera la generación de código.

✅ Mejora la calidad mediante sugerencias de buenas prácticas.

✅ Ayuda en la documentación y pruebas.

✅ Incrementa la productividad del equipo.

✅ Facilita la comprensión del código existente.

---

# Consideraciones Importantes

GitHub Copilot es un asistente, no un reemplazo del desarrollador.

Siempre se recomienda:

* Revisar el código generado.
* Validar reglas de negocio.
* Aplicar revisiones de seguridad.
* Ejecutar pruebas antes de desplegar.
* Comprender el código antes de aceptarlo.

---

# Resultado Esperado

Al finalizar esta sección el participante comprenderá:

✅ Qué es GitHub Copilot.

✅ Cómo utilizar Copilot Chat.

✅ Cómo aprovechar el contexto mediante `@workspace`.

✅ Cómo utilizar `#file`.

✅ Cómo utilizar `#selection`.

✅ Cómo generar código, pruebas y documentación.

✅ Cómo GitHub Copilot puede acompañar todo el ciclo de desarrollo.

✅ Evolucionar la solución:

```text
Workshop.Seguros.API
```

incorporando nuevas entidades y relaciones del dominio de seguros.

Al finalizar esta sección, la solución podría tener una estructura similar a:

```text
Workshop.Seguros.API
│
├── Program.cs
├── appsettings.json
│
├── Entidades
│   ├── SolicitudSeguro.cs
│   ├── Cliente.cs
│   ├── Cobertura.cs
│   └── DocumentoAdjunto.cs
│
├── Endpoints
│   ├── ObtenerSolicitudesSeguro.cs
│   ├── ObtenerSolicitudSeguroPorId.cs
│   ├── CrearSolicitudSeguro.cs
│   ├── ActualizarSolicitudSeguro.cs
│   └── EliminarSolicitudSeguro.cs
│
└── Properties
```

# 3. Prompts Efectivos

## 🎯 Objetivo

Aprender a redactar instrucciones claras y estructuradas para obtener mejores resultados de GitHub Copilot y aprovechar al máximo la Inteligencia Artificial durante el desarrollo de software.

Durante esta sección continuaremos evolucionando la solución:

```text
Workshop.Seguros.API
```

relacionada con la administración de solicitudes de seguros.

---

# ¿Qué es un Prompt?

Un prompt es la instrucción que se proporciona a la IA para solicitar una tarea.

La calidad del resultado depende en gran medida de la calidad del prompt.

```text
Mejor Prompt
      ↓
Más Contexto
      ↓
Menos Ambigüedad
      ↓
Mejor Resultado
```

La IA no adivina requerimientos.

La IA responde en función de la información que recibe.

---

# Los Prompts son Especificaciones

En desarrollo de software estamos acostumbrados a trabajar con requisitos.

Un prompt puede verse como una pequeña especificación funcional para la IA.

Mientras más claro sea el requerimiento:

* Mejor será la respuesta.
* Menos iteraciones serán necesarias.
* Menos correcciones habrá que realizar.

---

# Evolución de un Prompt

## Nivel 1: Prompt Deficiente

```text
Crea una API.
```

### Problemas

❌ No indica tecnología.

❌ No define arquitectura.

❌ No especifica el dominio del negocio.

❌ No establece restricciones.

### Resultado

```text
Respuesta ambigua e impredecible.
```

---

## Nivel 2: Prompt Específico

```text
Crea una API REST en .NET 8 para administrar solicitudes relacionadas con seguros.
```

### Ahora GitHub Copilot conoce:

✅ Tecnología.

✅ Tipo de aplicación.

✅ Dominio del negocio.

### Resultado

```text
Respuesta más precisa.
```

---

## Nivel 3: Prompt Estructurado

```text
Actúa como Arquitecto de Software.

Objetivo:
Diseñar una API REST para administrar solicitudes relacionadas con seguros.

Contexto:
La aplicación será utilizada por colaboradores de una organización.

Restricciones:

- .NET 8.
- Minimal API.
- Clean Architecture.
- XUnit.
- Comentarios en español.

Resultado esperado:

Generar entidades, endpoints y pruebas unitarias.
```

### Resultado

```text
Respuesta mucho más consistente y alineada al objetivo.
```

---

# Componentes de un Buen Prompt

## 1. Rol

Ejemplos:

```text
Actúa como Arquitecto de Software.
```

```text
Actúa como Desarrollador Senior .NET.
```

```text
Actúa como Especialista QA.
```

```text
Actúa como Especialista en Seguridad.
```

---

## 2. Objetivo

Ejemplo:

```text
Diseñar una API para administrar solicitudes de seguros.
```

---

## 3. Contexto

Ejemplo:

```text
La aplicación será utilizada por colaboradores de una organización y administrará solicitudes de seguros.
```

---

## 4. Restricciones

Ejemplo:

```text
- Utilizar .NET 8.
- Aplicar Clean Architecture.
- Generar comentarios en español.
- Utilizar XUnit para las pruebas.
```

---

## 5. Resultado Esperado

Ejemplo:

```text
Generar:

- Entidades.
- DTOs.
- Endpoints.
- Validaciones.
- Pruebas unitarias.
- Documentación.
```

---

# Plantilla Recomendada

```text
Actúa como [ROL].

Objetivo:
[OBJETIVO]

Contexto:
[CONTEXTO]

Restricciones:
[RESTRICCIONES]

Resultado esperado:
[SALIDA_DESEADA]
```

---

# Ingeniería de Prompts

Un prompt bien construido normalmente contiene cinco elementos:

```text
Rol
↓
Objetivo
↓
Contexto
↓
Restricciones
↓
Resultado esperado
```

No se trata de "hacer preguntas bonitas".

Se trata de comunicar correctamente los requerimientos a la IA.

---

# Regla de Oro

> La IA no reemplaza la capacidad de análisis del desarrollador.

```text
Garbage In
     ↓
Garbage Out
```

(Basura entra, basura sale).

---

# Ejercicios Prácticos

En esta sección construiremos la primera funcionalidad completa de la solución:

```text
Registrar una Solicitud de Seguro
```

---

## Ejercicio 1 - Prompt Deficiente

Solicitar a GitHub Copilot:

```text
Crea un endpoint.
```

Analizar la respuesta obtenida.

---

## Ejercicio 2 - Prompt Específico

Solicitar:

```text
Crea un endpoint REST en .NET 8 para registrar una solicitud de seguro.
```

Comparar los resultados con el ejercicio anterior.

---

## Ejercicio 3 - Prompt Estructurado

Solicitar:

```text
Actúa como Arquitecto de Software.

Objetivo:
Diseñar un endpoint para registrar una solicitud de seguro.

Contexto:
La solución Workshop.Seguros.API pertenece a un dominio empresarial.

Restricciones:

- Utilizar .NET 8.
- Minimal API.
- Clean Architecture.
- XUnit.
- Comentarios en español.

Resultado esperado:

Generar:

- Request.
- Response.
- Endpoint.
- Validaciones.
- Pruebas unitarias.
```

Comparar nuevamente los resultados.

---

## Ejercicio 4 - Generación de una Entidad

Solicitar:

```text
Actúa como Desarrollador Senior .NET.

Objetivo:
Crear la entidad Beneficiario.

Contexto:
La solución Workshop.Seguros.API administra solicitudes de seguros.

Restricciones:

- Utilizar C# y .NET 8.
- Agregar comentarios XML.
- Utilizar nombres descriptivos.
- Incluir validaciones básicas.

Resultado esperado:

Generar una entidad empresarial lista para producción.
```

---

## Ejercicio 5 - Generación de Pruebas Unitarias

Solicitar:

```text
Actúa como Especialista QA.

Objetivo:
Generar pruebas unitarias para la entidad Beneficiario.

Contexto:
La solución utiliza XUnit.

Resultado esperado:

Generar escenarios positivos, negativos y validaciones.
```

---

# Buenas Prácticas

✅ Proporcionar contexto.

✅ Definir claramente el objetivo.

✅ Especificar tecnologías.

✅ Indicar restricciones.

✅ Definir el resultado esperado.

✅ Dividir problemas complejos en tareas pequeñas.

✅ Refinar el prompt de forma iterativa.

✅ Validar siempre el resultado generado.

---

# Errores Comunes

❌ Prompts demasiado generales.

❌ Falta de contexto.

❌ No especificar tecnologías.

❌ Esperar que la IA adivine requerimientos.

❌ Pedir demasiadas cosas en una sola instrucción.

❌ Aceptar respuestas sin revisarlas.

---

# Resultado Esperado

Al finalizar esta sección el participante será capaz de:

✅ Construir prompts estructurados.

✅ Reducir iteraciones innecesarias.

✅ Obtener respuestas más precisas.

✅ Aprovechar mejor GitHub Copilot durante el desarrollo.

✅ Comprender que un prompt es una especificación para la IA y no simplemente una pregunta.

✅ Evolucionar la solución Workshop.Seguros.API incorporando nuevas funcionalidades.

✅ Comprender que la calidad del resultado depende directamente de la calidad de las instrucciones proporcionadas a la IA.


# 4. Agentes, Instructions y Skills

## 🎯 Objetivo

Comprender cómo personalizar GitHub Copilot mediante Agentes, Instructions y Skills, y aprender a utilizar la Inteligencia Artificial para crear y configurar estos elementos de forma más eficiente.

Durante esta sección continuaremos evolucionando la solución:

```text
Workshop.Seguros.API
```

y aprenderemos cómo especializar GitHub Copilot para adaptarlo a las necesidades de un equipo de desarrollo moderno.

---

# Del Prompt al Agente

Hasta este momento hemos trabajado utilizando GitHub Copilot con el comportamiento predeterminado.

Sin embargo, conforme los proyectos crecen y los equipos establecen estándares, resulta conveniente especializar el comportamiento de la IA.

En lugar de repetir constantemente las mismas instrucciones, es posible crear Agentes personalizados.

---

# ¿Qué es un Agente?

Un Agente es una configuración especializada que permite adaptar GitHub Copilot a un rol o escenario específico.

Puede verse como un miembro virtual del equipo.

Ejemplos:

* Arquitecto de Software.
* Desarrollador Backend.
* Especialista QA.
* Analista de Negocio.
* Especialista en Seguridad.
* Revisor de Código.
* Especialista DevOps.

---

# Componentes de un Agente

Un agente está compuesto principalmente por:

## Agente

Representa el propósito principal.

Ejemplo:

```text
Especialista Backend .NET
```

---

## Instructions

Son las reglas permanentes que debe seguir el agente.

Ejemplo:

```text
- Responde en español.
- Utiliza .NET 8.
- Aplica Clean Architecture.
- Sugiere pruebas unitarias con XUnit.
- Prioriza la mantenibilidad.
- Sigue buenas prácticas de seguridad.
```

---

## Skills

Representan conocimientos especializados que complementan al agente.

Ejemplos:

* Diseño de APIs REST.
* Patrones de diseño.
* Pruebas unitarias.
* Seguridad.
* Revisión de código.
* Documentación técnica.

---

# Arquitectura Conceptual

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
   │
   ▼
Modelo de IA
```

---

# Beneficios de Utilizar Agentes

Los agentes permiten:

✅ Obtener respuestas más consistentes.

✅ Reducir instrucciones repetitivas.

✅ Aplicar estándares del equipo.

✅ Reutilizar conocimiento.

✅ Incrementar la productividad.

✅ Facilitar la incorporación de nuevos desarrolladores.

---

# Utilizando la IA para Crear un Agente

Al igual que aprendimos a construir prompts efectivos, también podemos utilizar la IA para diseñar nuestros propios agentes.

Por ejemplo, podríamos solicitar:

```text
Actúa como experto en GitHub Copilot.

Objetivo:
Crear un agente especializado para un equipo Backend .NET.

Contexto:
El equipo desarrolla APIs empresariales utilizando .NET.

Resultado esperado:

Generar:

1. Nombre del agente.
2. Descripción.
3. Instructions recomendadas.
4. Skills recomendados.
```

---

# Caso Práctico del Taller

Supongamos que el equipo desea estandarizar la forma en que se desarrollan los servicios Backend.

En lugar de repetir instrucciones constantemente, se crea un agente especializado.

---

# Nombre del Agente

```text
Especialista Backend .NET
```

---

# Descripción

```text
Agente especializado en el desarrollo de APIs empresariales utilizando .NET y aplicando principios de Clean Architecture y buenas prácticas de ingeniería de software.
```

---

# Instructions

```text
- Responde en español.

- Utiliza .NET 8.

- Aplica principios de Clean Architecture.

- Sugiere pruebas unitarias utilizando XUnit.

- Prioriza código mantenible y desacoplado.

- Utiliza nombres descriptivos.

- Genera comentarios XML cuando sea apropiado.

- Aplica buenas prácticas de seguridad.

- Sugiere validaciones de negocio.

- Propón alternativas cuando existan varias opciones.

- Sigue principios SOLID y Clean Code.

- Explica las decisiones de diseño cuando sea necesario.
```

---

# Skills

```text
- Diseño de APIs REST.

- Clean Architecture.

- C# y .NET 8.

- Minimal APIs.

- Pruebas Unitarias con XUnit.

- Validaciones de negocio.

- Documentación técnica.

- Revisión de código.

- Principios SOLID.

- Clean Code.
```

---

# Crear un Agente en GitHub Copilot

## Paso 1

Abrir GitHub Copilot.

---

## Paso 2

Seleccionar:

```text
Agents
```

---

## Paso 3

Crear un nuevo agente.

---

## Paso 4

Definir:

* Nombre.
* Descripción.
* Instructions.

---

## Paso 5

Agregar los Skills correspondientes.

---

## Paso 6

Guardar el agente y comenzar a utilizarlo.

---

# Ejercicio Práctico 1

Solicitar a GitHub Copilot:

```text
Actúa como experto en GitHub Copilot.

Objetivo:
Crear un agente especializado para QA.

Contexto:
La solución Workshop.Seguros.API utiliza .NET 8 y XUnit.

Resultado esperado:

Generar:

1. Nombre del agente.
2. Descripción.
3. Instructions.
4. Skills.
```

---

# Posible Resultado

## Nombre

```text
Especialista QA .NET
```

---

## Instructions

```text
- Responde en español.
- Prioriza la calidad del software.
- Sugiere pruebas unitarias y de integración.
- Promueve alta cobertura de código.
- Sigue buenas prácticas de automatización.
```

---

## Skills

```text
- Pruebas Unitarias.
- Pruebas de Integración.
- Cobertura de Código.
- Automatización.
- Revisión de Calidad.
```

---

# Ejercicio Práctico 2

Utilizando el agente:

```text
Especialista Backend .NET
```

realizar la siguiente consulta:

```text
Necesito implementar la funcionalidad para registrar una solicitud de seguro.
```

Analizar cómo las respuestas ya incorporan automáticamente:

* .NET 8.
* Clean Architecture.
* Buenas prácticas.
* Validaciones.
* XUnit.
* Código mantenible.

sin necesidad de repetir dichas instrucciones.

---

# Casos de Uso Empresariales

Dentro de una organización podrían existir agentes especializados como:

| Agente                 | Propósito                            |
| ---------------------- | ------------------------------------ |
| Arquitecto de Software | Diseño de soluciones                 |
| Backend .NET           | Implementación de servicios          |
| Especialista QA        | Calidad y automatización             |
| Especialista Seguridad | Revisión de vulnerabilidades         |
| Analista de Negocio    | Historias de usuario y documentación |
| DevOps                 | Pipelines y despliegues              |
| Revisor de Código      | Calidad y mantenibilidad             |

---

# Reflexión

Los prompts efectivos del apartado anterior permiten obtener mejores resultados.

Los Agentes permiten llevar esos prompts a otro nivel.

En lugar de repetir constantemente:

```text
- Utiliza .NET 8.
- Aplica Clean Architecture.
- Sugiere pruebas unitarias.
- Responde en español.
```

estas instrucciones pasan a formar parte del comportamiento permanente del agente.

---

# Resultado Esperado

Al finalizar esta sección el participante será capaz de:

✅ Comprender qué es un Agente.

✅ Comprender el propósito de las Instructions.

✅ Comprender el propósito de los Skills.

✅ Crear agentes personalizados.

✅ Utilizar la IA para generar y configurar agentes.

✅ Adaptar GitHub Copilot a las necesidades del equipo.

✅ Estandarizar el desarrollo de software mediante agentes especializados.

✅ Comprender cómo un agente puede convertirse en un miembro virtual del equipo.


# 5. Caso Práctico

## 🎯 Objetivo

Demostrar cómo un Agente especializado puede ayudar a resolver una necesidad real de desarrollo de software aplicando automáticamente buenas prácticas, lineamientos y estándares definidos por el equipo.

Durante esta sección continuaremos evolucionando la solución:

```text
Workshop.Seguros.API
```

relacionada con la administración de solicitudes de seguros.

---

# Escenario

La organización necesita desarrollar una nueva funcionalidad para registrar solicitudes de seguros.

La organización ha definido los siguientes estándares:

* Desarrollo en .NET 8.
* Uso de Clean Architecture.
* Implementación de pruebas unitarias con XUnit.
* Documentación de endpoints.
* Buenas prácticas de seguridad.
* Código mantenible y desacoplado.

El objetivo es evitar que cada desarrollador tenga que recordar y especificar estos requisitos manualmente en cada consulta.

---

# Solución Tradicional

Un desarrollador podría realizar una consulta como:

```text
Genera una API para registrar solicitudes de seguros.
```

Sin embargo, el resultado dependerá completamente del contexto disponible y podría no seguir los estándares definidos por el equipo.

---

# Solución Utilizando un Agente

Se utilizará el agente creado en la sección anterior:

```text
Especialista Backend .NET
```

---

# Instructions del Agente

```text
Eres un Especialista Backend .NET.

Debes responder en español.

Debes utilizar .NET 8.

Debes aplicar Clean Architecture.

Debes sugerir pruebas unitarias utilizando XUnit.

Debes aplicar buenas prácticas de seguridad.

Debes generar soluciones mantenibles y escalables.

Debes seguir principios SOLID y Clean Code.
```

---

# Skills del Agente

```text
Diseño de APIs REST

Clean Architecture

C# y .NET 8

Minimal APIs

Pruebas Unitarias

Validaciones de negocio

Documentación técnica

Seguridad

Revisión de código
```

---

# Necesidad de Negocio

Registrar una solicitud de seguro.

---

# Información de la Solicitud

La solicitud debe almacenar:

* Número de solicitud.
* Identificación del cliente.
* Nombre del cliente.
* Fecha de creación.
* Tipo de seguro.
* Estado.
* Observaciones.

---

# Consulta Realizada al Agente

```text
Necesito implementar la funcionalidad para registrar una solicitud de seguro.

Genera:

- Entidad.
- DTOs.
- Endpoint.
- Validaciones.
- Pruebas unitarias.
```

---

# Resultado Esperado

El agente podría proponer la siguiente arquitectura:

## Dominio

```text
SolicitudSeguro
```

---

## Aplicación

```text
CrearSolicitudSeguroRequest

CrearSolicitudSeguroResponse

ValidadorCrearSolicitudSeguro
```

---

## API

```text
CrearSolicitudSeguroEndpoint
```

---

## Infraestructura

```text
RepositorioSolicitudSeguro
```

---

# Endpoint Propuesto

```http
POST /api/solicitudes-seguro
```

---

# Operaciones Futuras

```http
GET     /api/solicitudes-seguro

GET     /api/solicitudes-seguro/{id}

POST    /api/solicitudes-seguro

PUT     /api/solicitudes-seguro/{id}

DELETE  /api/solicitudes-seguro/{id}
```

---

# Validaciones de Negocio

El agente podría sugerir:

* Número de solicitud obligatorio.
* Identificación del cliente obligatoria.
* Nombre del cliente obligatorio.
* El tipo de seguro es obligatorio.
* La fecha de creación no puede ser futura.
* El estado inicial debe ser Pendiente.

---

# Pruebas Unitarias

El agente podría proponer:

## Casos positivos

* Crear una solicitud válida.

## Casos negativos

* Número de solicitud vacío.
* Identificación vacía.
* Nombre vacío.
* Tipo de seguro vacío.
* Fecha futura.

## Validaciones

* Estado inicial Pendiente.
* Valores obligatorios.

---

# Seguridad

El agente también podría sugerir:

* Validación de entradas.
* Manejo centralizado de excepciones.
* Autenticación.
* Autorización.
* Registro de eventos mediante logs.
* Evitar exponer información sensible.

---

# Documentación

El agente puede generar automáticamente:

* Comentarios XML.
* Documentación de endpoints.
* Ejemplos de requests.
* Ejemplos de responses.

---

# Beneficios Obtenidos

## Sin Agente

* Cada desarrollador realiza consultas diferentes.
* Resultados inconsistentes.
* Mayor riesgo de incumplir estándares.
* Mayor esfuerzo manual.

---

## Con Agente

* Respuestas alineadas con la organización.
* Menor esfuerzo de configuración.
* Mayor consistencia.
* Mejor calidad técnica.
* Menor curva de aprendizaje.
* Reutilización del conocimiento del equipo.

---

# Discusión

Analice con el grupo:

## ¿Qué otros agentes podrían existir?

### Arquitecto de Software

Encargado de:

* Diseño de soluciones.
* Patrones de diseño.
* Decisiones arquitectónicas.

---

### Especialista QA

Encargado de:

* Pruebas unitarias.
* Cobertura.
* Casos de prueba.

---

### Especialista Seguridad

Encargado de:

* Vulnerabilidades.
* OWASP.
* Validaciones.

---

### Analista de Negocio

Encargado de:

* Historias de usuario.
* Criterios de aceptación.
* Documentación funcional.

---

### DevOps

Encargado de:

* Pipelines.
* Docker.
* CI/CD.

---

### Revisor de Código

Encargado de:

* Calidad.
* Mantenibilidad.
* Principios SOLID.

---

# Flujo Completo

```text
Necesidad del Negocio
          │
          ▼
Especialista Backend .NET
          │
          ▼
GitHub Copilot
          │
          ▼
Entidad
DTOs
Endpoints
Validaciones
Pruebas Unitarias
Documentación
          │
          ▼
Workshop.Seguros.API
```

---

# Resultado Esperado

Al finalizar este ejercicio el participante comprenderá:

✅ Cómo un agente puede especializar el comportamiento de GitHub Copilot.

✅ Cómo las Instructions influyen en las respuestas.

✅ Cómo los Skills aportan capacidades especializadas.

✅ Cómo los agentes ayudan a estandarizar el desarrollo dentro de una organización.

✅ Cómo GitHub Copilot puede acompañar todo el ciclo de desarrollo de una funcionalidad real.

✅ Cómo reutilizar el conocimiento del equipo mediante agentes especializados.

✅ Cómo evolucionar progresivamente una solución empresarial utilizando IA.


# 6. Buenas Prácticas y Uso Empresarial

## 🎯 Objetivo

Conocer las principales recomendaciones para utilizar GitHub Copilot de forma segura, responsable y efectiva dentro de entornos empresariales.

Durante esta sección utilizaremos como referencia la solución:

```text
Workshop.Seguros.API
```

y el agente:

```text
Especialista Backend .NET
```

desarrollados a lo largo del workshop.

---

# GitHub Copilot como Asistente

Es importante comprender que GitHub Copilot es un asistente para el desarrollo de software.

Su propósito es ayudar a los desarrolladores a:

* Generar código.
* Resolver dudas técnicas.
* Crear documentación.
* Generar pruebas.
* Explicar código existente.
* Acelerar tareas repetitivas.

Sin embargo, las decisiones finales continúan siendo responsabilidad del equipo de desarrollo.

---

# Principio Fundamental

> GitHub Copilot y los Agentes potencian las capacidades del desarrollador, pero no reemplazan su criterio técnico.

Todo código generado debe ser revisado antes de ser incorporado a una solución.

---

# Uso Responsable de la Inteligencia Artificial

La IA puede acelerar el trabajo, pero no debe sustituir:

* El análisis técnico.
* El diseño de arquitectura.
* La revisión de código.
* La validación funcional.
* Las pruebas.
* El criterio profesional.

---

# Seguridad de la Información

Antes de utilizar GitHub Copilot es importante considerar las políticas de seguridad de la organización.

---

## Evitar Compartir Información Sensible

No se recomienda incluir:

* Contraseñas.
* Tokens de acceso.
* Secretos de aplicaciones.
* Llaves criptográficas.
* Información confidencial de clientes.
* Datos personales sensibles.
* Información de producción.

### Incorrecto

```text
Mi contraseña de producción es...
```

```text
Este es el token de acceso del sistema...
```

```text
La cadena de conexión de la base de datos es...
```

---

## Buenas Prácticas

✅ Utilizar datos ficticios para ejemplos.

✅ Ocultar información sensible.

✅ Revisar las políticas internas de la organización.

✅ Utilizar variables de entorno y gestores de secretos.

---

# Validación del Código Generado

Aunque GitHub Copilot genera código funcional, siempre se recomienda validar:

* Correctitud funcional.
* Seguridad.
* Rendimiento.
* Escalabilidad.
* Cumplimiento de estándares internos.
* Reglas de negocio.

---

## Revisar Siempre

Antes de aceptar código generado:

* Comprender la solución propuesta.
* Verificar dependencias.
* Revisar excepciones y validaciones.
* Confirmar cumplimiento de reglas de negocio.
* Revisar el manejo de errores.
* Analizar posibles vulnerabilidades.

---

# Uso de Prompts Claros

Prompts bien estructurados producen mejores resultados.

---

### Poco claro

```text
Haz una API.
```

---

### Más efectivo

```text
Actúa como Desarrollador Senior .NET.

Objetivo:
Implementar un endpoint para registrar una solicitud de seguro.

Contexto:
La solución Workshop.Seguros.API utiliza .NET 8 y Clean Architecture.

Resultado esperado:
Generar endpoint, validaciones y pruebas unitarias.
```

---

# Mantener Consistencia

Cuando se trabaja en equipo es recomendable:

* Definir estándares.
* Compartir instrucciones comunes.
* Utilizar agentes especializados.
* Documentar lineamientos.
* Promover buenas prácticas.

Esto ayuda a obtener resultados más consistentes entre diferentes desarrolladores.

---

# Agentes como Conocimiento Compartido

Los agentes permiten reutilizar el conocimiento del equipo.

Por ejemplo:

```text
Especialista Backend .NET
```

puede incorporar automáticamente:

* .NET 8.
* Clean Architecture.
* SOLID.
* Clean Code.
* XUnit.
* Buenas prácticas de seguridad.

De esta forma los desarrolladores no necesitan repetir constantemente las mismas instrucciones.

---

# Revisión de Código

El código generado por GitHub Copilot debe seguir el mismo proceso de revisión que cualquier otro desarrollo.

Se recomienda:

* Pull Requests.
* Code Reviews.
* Pruebas unitarias.
* Pruebas de integración.
* Validaciones de seguridad.

---

# Integración con el Ciclo de Desarrollo

La Inteligencia Artificial no reemplaza las prácticas tradicionales de ingeniería.

Por el contrario, se integra con ellas.

```text
Requerimiento
      │
      ▼
GitHub Copilot y Agentes
      │
      ▼
Desarrollo
      │
      ▼
Pruebas
      │
      ▼
Pull Request
      │
      ▼
Code Review
      │
      ▼
Despliegue
```

---

# Medición del Valor

GitHub Copilot debe considerarse una herramienta de productividad.

Algunas métricas que pueden analizarse son:

* Tiempo de desarrollo.
* Reducción de tareas repetitivas.
* Velocidad de generación de pruebas.
* Velocidad de documentación.
* Productividad del equipo.
* Reducción del tiempo de aprendizaje.

---

# Casos de Uso Recomendados

GitHub Copilot suele aportar mayor valor en:

## Desarrollo

* Generación de código.
* Refactorización.
* Creación de APIs.
* Consultas SQL.
* Scripts.

---

## Calidad

* Pruebas unitarias.
* Pruebas de integración.
* Casos de prueba.

---

## Documentación

* Comentarios XML.
* Documentación técnica.
* Historias de usuario.
* Diagramas y descripciones.

---

## Aprendizaje

* Nuevos lenguajes.
* Nuevos frameworks.
* Patrones de diseño.
* Buenas prácticas.

---

# Casos Donde Se Debe Tener Mayor Cuidado

Se recomienda una revisión más rigurosa cuando el código involucra:

* Seguridad.
* Autenticación.
* Autorización.
* Criptografía.
* Procesamiento financiero.
* Datos sensibles.
* Integraciones críticas.
* Información de clientes.

---

# Recomendaciones para Equipos

## Hacer

✅ Utilizar GitHub Copilot como apoyo.

✅ Validar el código generado.

✅ Aplicar revisiones de código.

✅ Compartir buenas prácticas.

✅ Utilizar prompts claros.

✅ Definir estándares comunes.

✅ Crear agentes especializados.

✅ Promover la colaboración entre equipos.

---

## Evitar

❌ Confiar ciegamente en las respuestas.

❌ Compartir información sensible.

❌ Omitir pruebas.

❌ Omitir revisiones de seguridad.

❌ Incorporar código sin comprenderlo.

❌ Saltarse los procesos de revisión.

---

# Reflexión

La adopción de la Inteligencia Artificial no consiste únicamente en generar código más rápido.

Su verdadero valor está en:

* Compartir conocimiento.
* Estandarizar prácticas.
* Mejorar la calidad.
* Reducir tareas repetitivas.
* Incrementar la productividad del equipo.

---

# Idea Clave

> La Inteligencia Artificial no reemplaza la ingeniería de software; la potencia.

---

# Resultado Esperado

Al finalizar esta sección el participante comprenderá:

✅ Cómo utilizar GitHub Copilot de forma responsable.

✅ Qué información no debe compartirse.

✅ La importancia de validar el código generado.

✅ Cómo integrar GitHub Copilot dentro de los procesos de desarrollo existentes.

✅ Cómo aprovechar los agentes para compartir conocimiento.

✅ Cómo utilizar la Inteligencia Artificial dentro de un entorno empresarial.

✅ Que la IA no reemplaza las buenas prácticas de ingeniería, sino que ayuda a aplicarlas de forma más consistente.


# 7. Conclusiones

## 🎯 Objetivo

Recapitular los principales conceptos vistos durante el taller y establecer una ruta de adopción para comenzar a utilizar GitHub Copilot y los Agentes de forma efectiva en el trabajo diario.

---

# El Recorrido del Taller

Durante este workshop no solo aprendimos conceptos aislados.

A lo largo de las diferentes secciones fuimos construyendo y evolucionando una solución empresarial:

```text id="lhx6h5"
Workshop.Seguros.API
```

Esto permitió experimentar cómo GitHub Copilot puede acompañar al desarrollador durante todo el ciclo de vida del software.

---

# ¿Qué Aprendimos?

## Configuración del Entorno

Se configuró Visual Studio Code para trabajar con Inteligencia Artificial.

Se instalaron y configuraron:

* GitHub Copilot.
* GitHub Copilot Chat.
* Extensiones para desarrollo moderno.

---

## Uso de GitHub Copilot

Se exploraron los diferentes modos de interacción disponibles:

* Ask.
* Plan.
* Agent.

---

## Prompts Efectivos

Se comprobó cómo la calidad de los resultados depende directamente de la calidad de las instrucciones proporcionadas.

Se analizaron elementos como:

* Rol.
* Objetivo.
* Contexto.
* Restricciones.
* Resultado esperado.

---

## Agentes, Instructions y Skills

Se comprendió cómo especializar el comportamiento de GitHub Copilot mediante:

* Agentes.
* Instructions.
* Skills.

Permitiendo respuestas más consistentes y alineadas con los estándares del equipo.

---

## Caso Práctico

Se utilizó un agente especializado para desarrollar una funcionalidad real de la solución.

Esto permitió observar cómo la IA puede participar en:

* Diseño.
* Implementación.
* Validaciones.
* Pruebas.
* Documentación.

---

## Buenas Prácticas y Uso Empresarial

Se revisaron aspectos relacionados con:

* Seguridad.
* Calidad.
* Gobierno.
* Uso responsable de la Inteligencia Artificial.

---

# Evolución de la Solución

A lo largo del taller, la solución fue creciendo progresivamente:

## Sección 1

```text id="v7g84q"
Workshop.Seguros.API
```

Se configuró el entorno de trabajo.

---

## Sección 2

Se incorporaron las primeras entidades:

```text id="f38k2j"
SolicitudSeguro
Cliente
Cobertura
DocumentoAdjunto
```

---

## Sección 3

Se aprendió a construir mejores prompts y a obtener resultados más precisos.

---

## Sección 4

Se crearon agentes especializados para incorporar conocimiento y estándares del equipo.

---

## Sección 5

Se desarrolló una funcionalidad real utilizando un agente especializado.

---

## Sección 6

Se analizaron buenas prácticas para el uso empresarial de la Inteligencia Artificial.

---

# Principales Mensajes

## GitHub Copilot es un Asistente

GitHub Copilot ayuda a acelerar el trabajo del desarrollador, pero no reemplaza:

* El análisis técnico.
* La experiencia.
* El criterio profesional.
* La responsabilidad sobre el software construido.

---

## La Calidad del Resultado Depende del Contexto

Mientras mejor sea el prompt, mejor será el resultado.

La IA necesita contexto para generar respuestas más precisas y útiles.

---

## Los Agentes Permiten Escalar el Uso de la IA

Los agentes permiten incorporar:

* Estándares.
* Buenas prácticas.
* Conocimiento organizacional.
* Consistencia entre equipos.

---

## La IA Debe Integrarse al Proceso de Desarrollo

La Inteligencia Artificial no reemplaza las prácticas tradicionales de ingeniería.

Por el contrario, las complementa.

```text id="h7rxli"
Requerimiento
      │
      ▼
GitHub Copilot y Agentes
      │
      ▼
Desarrollo
      │
      ▼
Pruebas
      │
      ▼
Pull Request
      │
      ▼
Code Review
      │
      ▼
Despliegue
```

---

# ¿Qué Puedo Hacer Mañana?

## Nivel 1

Utilizar GitHub Copilot para:

* Generar código repetitivo.
* Crear pruebas unitarias.
* Generar documentación.

---

## Nivel 2

Utilizar prompts más estructurados incorporando:

* Rol.
* Objetivo.
* Contexto.
* Restricciones.
* Resultado esperado.

---

## Nivel 3

Crear agentes especializados para diferentes necesidades:

* Arquitectura.
* Backend.
* QA.
* Seguridad.
* DevOps.
* Documentación.

---

## Nivel 4

Compartir esos agentes con el equipo y convertirlos en una forma de reutilizar conocimiento.

---

## Nivel 5

Incorporar la Inteligencia Artificial al ciclo completo de desarrollo.

---

# Próximos Pasos

Una vez dominados estos conceptos, es posible avanzar hacia escenarios más avanzados:

* Agentes empresariales.
* Automatización de procesos.
* Integración con herramientas corporativas.
* Desarrollo asistido por IA.
* Ingeniería de Software impulsada por IA.
* Agentes especializados por dominio del negocio.

---

# Reflexión Final

> La Inteligencia Artificial no reemplaza a los desarrolladores; potencia sus capacidades.

Las organizaciones que logren combinar:

* La experiencia de sus equipos.
* El conocimiento del negocio.
* Las buenas prácticas de ingeniería.
* El uso adecuado de la Inteligencia Artificial.

estarán mejor preparadas para desarrollar soluciones de mayor calidad, en menor tiempo y con mayor capacidad de adaptación.

---

# Idea Final

```text id="7q6v6m"
La ventaja competitiva no está en tener IA.

La ventaja competitiva está en cómo las organizaciones combinan:

Personas + Conocimiento + Ingeniería + Inteligencia Artificial
```

---

# ¡Gracias por Participar!

## Preguntas y Respuestas

Espacio abierto para consultas, comentarios y experiencias relacionadas con GitHub Copilot, Agentes e Inteligencia Artificial aplicada al desarrollo de software.
