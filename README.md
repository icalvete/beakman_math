# Mi mundo de Beakman (MATEMATICAS)

<p align="center">
  <img src="gpt/logo.jpeg" alt="Beakman" width="200"/>
</p>

<p align="center">
  <em>GPT personalizado para enseñar Matemáticas de 1º de la ESO</em><br>
  <em>Inspirado en el estilo de Beakman: curioso, divertido y reflexivo</em>
</p>

---

## Qué es este proyecto

Un tutor de matemáticas basado en ChatGPT diseñado para estudiantes de 12 años (1º de la ESO en España). El GPT adopta la personalidad de Beakman, el famoso científico televisivo, y prioriza que el alumno **entienda** las matemáticas, no solo que memorice fórmulas.

**Público objetivo:** Profesores, familias y uso educativo supervisado.

---

## Cómo crear tu propio GPT

Sigue estos pasos para crear tu propia copia de este GPT. No necesitas conocimientos técnicos, solo una cuenta de ChatGPT Plus.

### Requisitos previos

- **Cuenta de ChatGPT Plus** ($20/mes) - Los GPTs personalizados solo están disponibles para usuarios de pago
- **Navegador web** - Chrome, Firefox, Safari o Edge
- **Los archivos de este repositorio** - Descárgalos o clona el repositorio

### Paso 1: Acceder al GPT Builder

1. Abre tu navegador y ve a: **https://chat.openai.com**
2. Inicia sesión con tu cuenta de ChatGPT Plus
3. En el menú lateral izquierdo, haz clic en **"Explore GPTs"**
4. En la esquina superior derecha, haz clic en **"Create"**
5. Se abrirá el editor de GPTs con dos pestañas: "Create" y "Configure"
6. Haz clic en la pestaña **"Configure"** (la usaremos para configurar todo manualmente)

### Paso 2: Información básica

En la pestaña "Configure", rellena los siguientes campos:

**Name (Nombre):**
```
Mi mundo de Beakman (MATEMATICAS)
```

**Description (Descripción):**
```
Guía interactiva para enseñar y explorar Matemáticas. Inspirado en el estilo de Beakman: curioso, divertido y reflexivo. Diseñado para profesores, familias y uso educativo supervisado.
```

**Profile Picture (Imagen de perfil):**
1. Haz clic en el icono de imagen
2. Selecciona "Upload a photo"
3. Busca y selecciona el archivo `gpt/logo.jpeg` de este repositorio

### Paso 3: Instrucciones (el cerebro del GPT)

El campo **Instructions** es donde defines cómo se comportará el GPT. Aquí es donde copiarás el prompt principal.

1. Abre el archivo `gpt/Curso_Matematicas_1ESO_Prompt.txt` con cualquier editor de texto (Bloc de notas, TextEdit, etc.)
2. Selecciona **todo el contenido** (Ctrl+A o Cmd+A)
3. Cópialo (Ctrl+C o Cmd+C)
4. En el GPT Builder, haz clic en el campo "Instructions"
5. Pega el contenido (Ctrl+V o Cmd+V)

**¿Por qué es importante este archivo?**

El prompt de instrucciones define:
- La personalidad del GPT (paciente, cercano, nunca ridiculiza)
- El método de enseñanza (visual primero, luego palabras, finalmente símbolos)
- Cómo gestionar bloqueos del alumno
- Qué comandos puede usar el estudiante

### Paso 4: Conversation starters (Iniciadores de conversación)

Los "Conversation starters" son botones que aparecen cuando el alumno abre el chat. Le ayudan a saber cómo empezar.

1. Busca la sección "Conversation starters"
2. Haz clic en "Add starter"
3. Escribe:
```
🧭 ¿Te has quedado en blanco o no sabes por dónde empezar? Escribe Ayuda y te guío paso a paso.
```

Puedes añadir más iniciadores si quieres (hasta 4), por ejemplo:
- `Quiero repasar fracciones`
- `No entiendo este ejercicio`
- `Dame un ejercicio de porcentajes`

### Paso 5: Knowledge (Base de conocimiento)

La sección **Knowledge** permite subir archivos que el GPT usará como referencia. Esto es fundamental para que las respuestas sean precisas y coherentes con el temario.

1. Busca la sección "Knowledge"
2. Haz clic en "Upload files"
3. Navega a la carpeta `knowledge/` de este repositorio
4. Selecciona **todos** los archivos `.txt`:
   - `00_Mapa_del_Curso_Matematicas.txt`
   - `01_Numeros_Naturales.txt`
   - `02_Divisibilidad.txt`
   - `03_Fracciones.txt`
   - `04_Decimales.txt`
   - `05_Fracciones_y_Decimales.txt`
   - `06_Porcentajes.txt`
   - `07_Algebra_Inicial.txt`
   - `08_Medida.txt`
   - `09_Geometria_Plana.txt`
   - `10_Estadistica_y_Probabilidad.txt`
5. Haz clic en "Open" o "Abrir"

**¿Por qué subir estos archivos?**

Sin Knowledge, el GPT improvisaría basándose en su conocimiento general, lo cual puede generar:
- Contenido no adaptado al nivel de 1º ESO
- Explicaciones inconsistentes entre sesiones
- Mayor riesgo de "alucinaciones" (inventar información)

Con Knowledge, el GPT consulta primero estos archivos y da respuestas coherentes con el temario definido.

### Paso 6: Capabilities (Capacidades)

Esta sección define qué herramientas adicionales puede usar el GPT.

Configuración recomendada:

| Capacidad | Activar | Razón |
|-----------|---------|-------|
| **Web Browsing** | ✅ Sí | Permite buscar información adicional en fuentes educativas cuando el Knowledge no es suficiente |
| **DALL-E Image Generation** | ⬜ Opcional | Puede generar diagramas, pero no es esencial |
| **Code Interpreter** | ⬜ No | No es necesario para matemáticas de este nivel |

### Paso 7: Guardar el GPT

1. Revisa que todos los campos estén completos
2. En la esquina superior derecha, haz clic en **"Create"** (o "Update" si estás editando)
3. Elige la visibilidad:
   - **Only me**: Solo tú puedes usarlo
   - **Anyone with the link**: Cualquiera con el enlace puede usarlo
   - **Public**: Aparece en la tienda de GPTs
4. Haz clic en "Save"

¡Listo! Tu GPT está creado y puedes empezar a usarlo.

---

## Protección contra alucinaciones y desinformación

Los modelos de lenguaje como GPT-4 pueden "alucinar", es decir, inventar información que parece correcta pero no lo es. En un contexto educativo, esto es especialmente peligroso.

Este GPT incluye varias capas de protección:

### 1. Knowledge como fuente principal

El prompt indica explícitamente:
> "Usa siempre los archivos de Knowledge como fuente principal."

Esto fuerza al GPT a consultar primero el contenido verificado antes de improvisar.

### 2. Autorización explícita para decir "no lo sé"

El prompt incluye:
> "Si no estás seguro: dilo, pide aclaraciones, no inventes datos ni ejemplos."

Los modelos de lenguaje tienden a dar siempre una respuesta, aunque no la sepan. Esta instrucción les da "permiso" para admitir desconocimiento, reduciendo las alucinaciones.

### 3. Limitación de fuentes externas

Cuando el GPT necesita buscar información adicional:
> "Usa solo fuentes educativas o institucionales fiables. Resume y adapta. Evita datos no contrastados."

Esto evita que el GPT cite fuentes dudosas o información no verificada.

### 4. Transparencia sobre limitaciones

El prompt indica:
> "Si falta contenido, indícalo y propone subir el archivo adecuado."

El GPT avisará cuando no tenga información suficiente en lugar de inventarla.

---

## Estructura del repositorio

```
/beakman_math
├── README.md                   # Este archivo (guía completa)
├── CLAUDE.md                   # Guía para asistentes de código
├── gpt/                        # Configuración del GPT
│   ├── logo.jpeg               # Imagen de perfil del GPT
│   └── Curso_Matematicas_1ESO_Prompt.txt    # Instrucciones principales
├── knowledge/                  # Archivos de Knowledge (subir al GPT)
│   ├── 00_Mapa_del_Curso_Matematicas.txt
│   ├── 01_Numeros_Naturales.txt
│   ├── 02_Divisibilidad.txt
│   ├── 03_Fracciones.txt
│   ├── 04_Decimales.txt
│   ├── 05_Fracciones_y_Decimales.txt
│   ├── 06_Porcentajes.txt
│   ├── 07_Algebra_Inicial.txt
│   ├── 08_Medida.txt
│   ├── 09_Geometria_Plana.txt
│   └── 10_Estadistica_y_Probabilidad.txt
└── docs/                       # Documentación técnica
    └── Curso_Matematicas_1ESO_Prompt_Comentado.txt
```

---

## Currículo incluido

El GPT cubre el temario completo de Matemáticas de 1º de la ESO:

| # | Tema | Descripción |
|---|------|-------------|
| 1 | Números Naturales | Contar, ordenar, operar |
| 2 | Divisibilidad | Múltiplos, divisores, MCD, mcm |
| 3 | Fracciones | Partes de una unidad |
| 4 | Decimales | Números con coma |
| 5 | Fracciones y Decimales | Conversión entre ambos |
| 6 | Porcentajes | Proporciones sobre 100 |
| 7 | Álgebra Inicial | Letras como números |
| 8 | Medida | Unidades y conversiones |
| 9 | Geometría Plana | Figuras en 2D |
| 10 | Estadística y Probabilidad | Datos y azar |

El orden es progresivo: cada tema se apoya en los anteriores.

---

## Comandos disponibles para el alumno

El estudiante puede escribir estos comandos en lenguaje natural (no hace falta escribirlos exactamente así):

| Comando | Qué hace |
|---------|----------|
| **Ayuda** | Guía paso a paso para empezar |
| **Mapa del curso** | Muestra todos los temas disponibles |
| **Siguiente tema** | Avanza al tema siguiente |
| **Tema anterior** | Vuelve al tema anterior |
| **Repaso rápido** | Resumen del tema actual |
| **Ejercicios guiados** | Práctica con ayuda del GPT |
| **Pensar sin calcular** | Ejercicios de razonamiento sin hacer cuentas |
| **Errores típicos** | Muestra los fallos más comunes |
| **Explica con ejemplo** | Pide un ejemplo práctico |
| **Explícamelo con un dibujo** | Pide una explicación visual |
| **Explícamelo como un esquema** | Pide un diagrama conceptual |
| **Consejo de estudio** | Tips para estudiar mejor |

---

## Filosofía pedagógica

El GPT sigue principios pedagógicos específicos. Cada uno tiene una razón técnica:

### 1. Comprensión antes que cálculo

> "Prioriza siempre comprensión, razonamiento, conexión con situaciones reales. Antes que memorizar reglas o aplicar pasos sin sentido."

**Por qué:** Los modelos de lenguaje son buenos generando procedimientos paso a paso, pero pueden hacerlo sin sentido. Esta instrucción fuerza explicaciones con significado.

### 2. Visual → Palabras → Símbolos

> "Explica siempre primero con imágenes mentales o esquemas. Después usa palabras sencillas. Finalmente introduce símbolos matemáticos."

**Por qué:** Evita la abstracción prematura. Los alumnos que ven símbolos antes de entender el concepto memorizan sin comprender.

### 3. El error es parte del aprendizaje

> "Nunca ridiculizas errores ni minimizas dificultades. Nunca digas que algo es fácil o evidente."

**Por qué:** Frases como "es fácil" generan ansiedad en alumnos que no lo entienden. Normalizar el error reduce bloqueos.

### 4. Estructura repetible

Cada explicación sigue el mismo patrón:
1. Introducción visual
2. Idea matemática central
3. Ejemplo cotidiano
4. Preguntas para pensar
5. Mini comprobación
6. Opciones para continuar

**Por qué:** La predictibilidad reduce la carga cognitiva. El alumno sabe qué esperar.

---

## Personalización

### Añadir más temas

1. Crea un nuevo archivo en `knowledge/` con el formato:

```
TEMA X – NOMBRE DEL TEMA

Descripción breve del tema.

Ideas clave:
- Punto 1
- Punto 2

Errores típicos:
- Error común 1

Relación con otros temas:
Conexión con temas anteriores/posteriores.
```

2. Sube el nuevo archivo al Knowledge del GPT en el GPT Builder

### Modificar el comportamiento

1. Edita `gpt/Curso_Matematicas_1ESO_Prompt.txt`
2. Consulta `docs/Curso_Matematicas_1ESO_Prompt_Comentado.txt` para entender el propósito de cada sección antes de modificar
3. Copia el nuevo contenido en el campo Instructions del GPT Builder

---

## Limitaciones conocidas

| Limitación | Descripción |
|------------|-------------|
| **Actualización manual** | Los cambios en este repositorio no se sincronizan automáticamente con el GPT. Debes actualizar manualmente en el GPT Builder. |
| **Tamaño de Knowledge** | OpenAI limita el tamaño de los archivos de Knowledge. Si añades mucho contenido, puede que necesites dividirlo. |
| **Sin historial entre sesiones** | El GPT no recuerda conversaciones anteriores. Cada chat empieza de cero. |
| **Dependencia de ChatGPT Plus** | Requiere suscripción de pago ($20/mes). |

---

## ⚠️ Descargo de responsabilidad

> **IMPORTANTE: Lee esto antes de usar el proyecto**
>
> Este proyecto se proporciona **"tal cual"**, sin garantías de ningún tipo.
>
> - Este GPT es una **herramienta de apoyo educativo**, no un sustituto de profesores, tutores o profesionales de la educación.
> - Las respuestas generadas por el GPT pueden contener **errores o imprecisiones**. A pesar de las medidas de protección implementadas, los modelos de lenguaje pueden "alucinar" (inventar información).
> - **Se recomienda supervisión adulta** durante el uso por parte de menores.
> - El autor **no se hace responsable** de:
>   - Errores en el contenido generado por el GPT
>   - Decisiones académicas tomadas basándose en las respuestas del GPT
>   - Cualquier perjuicio derivado del uso de este proyecto
> - La imagen utilizada (Beakman) es propiedad de sus respectivos titulares y se usa aquí con fines educativos y sin ánimo de lucro.
> - Este proyecto **no está afiliado** con OpenAI, ChatGPT, ni con los creadores originales del programa "El mundo de Beakman".
>
> **⚠️ Úsalo como complemento, nunca como única fuente de aprendizaje.**

---

## Licencia

Este proyecto está licenciado bajo **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**.

[![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

Esto significa que puedes:
- ✅ **Compartir** — copiar y redistribuir el material en cualquier medio o formato
- ✅ **Adaptar** — remezclar, transformar y construir sobre el material para cualquier propósito, incluso comercial

Con las siguientes condiciones:
- 📋 **Atribución** — Debes dar crédito apropiado, proporcionar un enlace a la licencia e indicar si se realizaron cambios
- 📋 **CompartirIgual** — Si remezclas, transformas o creas a partir del material, debes distribuir tu contribución bajo la misma licencia que el original

Ver el archivo [LICENSE](LICENSE) para más detalles.

---

<p align="center">
  <em>"Entender es más importante que acertar"</em>
</p>
