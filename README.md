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

> **Referencia rápida:** El archivo `gpt/configuracion.txt` contiene todos los textos listos para copiar y pegar en el editor de GPTs.

### Requisitos previos

- **Cuenta de ChatGPT Plus** ($20/mes) - Los GPTs personalizados solo están disponibles para usuarios de pago
- **Navegador web** - Chrome, Firefox, Safari o Edge
- **Los archivos de este repositorio** - Descárgalos o clona el repositorio

### Paso 1: Acceder al editor de GPTs

1. Abre tu navegador y ve a: **https://chat.openai.com**
2. Inicia sesión con tu cuenta de ChatGPT Plus
3. En el menú lateral izquierdo, haz clic en **"Explorar GPTs"**
4. En la esquina superior derecha, haz clic en **"Crear"**
5. Se abrirá el editor de GPTs con dos pestañas: "Crear" y "Configurar"
6. Haz clic en la pestaña **"Configurar"** (la usaremos para configurar todo manualmente)

### Paso 2: Información básica

En la pestaña "Configurar", rellena los siguientes campos:

**Nombre:**
```
Mi mundo de Beakman (MATEMATICAS)
```

**Descripción:**
```
Guía interactiva para enseñar y explorar Matemáticas. Inspirado en el estilo de Beakman: curioso, divertido y reflexivo. Diseñado para profesores, familias y uso educativo supervisado.
```

**Imagen de perfil:**
1. Haz clic en el icono de imagen
2. Selecciona "Subir una foto"
3. Busca y selecciona el archivo `gpt/logo.jpeg` de este repositorio

### Paso 3: Instrucciones (el cerebro del GPT)

El campo **Instrucciones** es donde defines cómo se comportará el GPT. Aquí es donde copiarás el prompt principal.

1. Abre el archivo `gpt/Curso_Matematicas_1ESO_Prompt.txt` con cualquier editor de texto (Bloc de notas, TextEdit, etc.)
2. Selecciona **todo el contenido** (Ctrl+A o Cmd+A)
3. Cópialo (Ctrl+C o Cmd+C)
4. En el editor de GPTs, haz clic en el campo "Instrucciones"
5. Pega el contenido (Ctrl+V o Cmd+V)

**¿Por qué es importante este archivo?**

El prompt de instrucciones define:
- La personalidad del GPT (paciente, cercano, nunca ridiculiza)
- El método de enseñanza (visual primero, luego palabras, finalmente símbolos)
- Cómo gestionar bloqueos del alumno
- Qué comandos puede usar el estudiante

### Paso 4: Iniciadores de conversación

Los "Iniciadores de conversación" son botones que aparecen cuando el alumno abre el chat. Le ayudan a saber cómo empezar.

1. Busca la sección "Iniciadores de conversación"
2. Haz clic en "Añadir iniciador" y escribe:

```
¿Te has quedado en blanco o no sabes por donde empezar? Escribe Ayuda y te guio paso a paso.
```

> **Nota:** Opcionalmente puedes anadir mas iniciadores como "Quiero repasar un tema", "No entiendo este ejercicio" o "Dame un ejercicio para practicar".

### Paso 5: Conocimiento (Base de conocimiento)

La sección **Conocimiento** permite subir archivos que el GPT usará como referencia. Esto es fundamental para que las respuestas sean precisas y coherentes con el temario.

1. Busca la sección "Conocimiento"
2. Haz clic en "Subir archivos"
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
5. Haz clic en "Abrir"

**¿Por qué subir estos archivos?**

Sin archivos de Conocimiento, el GPT improvisaría basándose en su conocimiento general, lo cual puede generar:
- Contenido no adaptado al nivel de 1º ESO
- Explicaciones inconsistentes entre sesiones
- Mayor riesgo de "alucinaciones" (inventar información)

Con archivos de Conocimiento, el GPT consulta primero estos archivos y da respuestas coherentes con el temario definido.

### Paso 6: Capacidades

Esta sección define qué herramientas adicionales puede usar el GPT.

Configuración recomendada:

| Capacidad | Activar | Razon |
|-----------|---------|-------|
| **Navegacion web** | Si | Permite buscar informacion adicional en fuentes educativas cuando el Conocimiento no es suficiente |
| **Generacion de imagenes (DALL-E)** | Opcional | Puede generar diagramas, pero no es esencial |
| **Interprete de codigo** | No | No es necesario para matematicas de este nivel |

### Paso 7: Guardar el GPT

1. Revisa que todos los campos estén completos
2. En la esquina superior derecha, haz clic en **"Crear"** (o **"Actualizar"** si estás editando)
3. Elige la visibilidad:
   - **Solo yo**: Solo tú puedes usarlo
   - **Cualquiera con el enlace**: Cualquiera con el enlace puede usarlo
   - **Público**: Aparece en la tienda de GPTs
4. Haz clic en "Guardar"

¡Listo! Tu GPT está creado y puedes empezar a usarlo.

---

## Protección contra alucinaciones y desinformación

Los modelos de lenguaje como GPT-4 pueden "alucinar", es decir, inventar información que parece correcta pero no lo es. En un contexto educativo, esto es especialmente peligroso.

Este GPT incluye varias capas de protección:

### 1. Conocimiento como fuente principal

El prompt indica explícitamente:
> "Usa siempre los archivos de Conocimiento como fuente principal."

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
│   ├── configuracion.txt       # Textos para copiar/pegar en el editor
│   ├── logo.jpeg               # Imagen de perfil del GPT
│   └── Curso_Matematicas_1ESO_Prompt.txt    # Instrucciones principales
├── knowledge/                  # Archivos de Conocimiento (subir al GPT)
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

2. Sube el nuevo archivo a la sección Conocimiento del GPT en el editor de GPTs

### Modificar el comportamiento

1. Edita `gpt/Curso_Matematicas_1ESO_Prompt.txt`
2. Consulta `docs/Curso_Matematicas_1ESO_Prompt_Comentado.txt` para entender el propósito de cada sección antes de modificar
3. Copia el nuevo contenido en el campo Instrucciones del editor de GPTs

---

## Limitaciones conocidas

| Limitación | Descripción |
|------------|-------------|
| **Actualización manual** | Los cambios en este repositorio no se sincronizan automáticamente con el GPT. Debes actualizar manualmente en el editor de GPTs. |
| **Tamaño de Conocimiento** | OpenAI limita el tamaño de los archivos de Conocimiento. Si añades mucho contenido, puede que necesites dividirlo. |
| **Sin historial entre sesiones** | El GPT no recuerda conversaciones anteriores. Cada chat empieza de cero. |
| **Dependencia de ChatGPT Plus** | Requiere suscripción de pago ($20/mes). |

---

## Descargo de responsabilidad

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
> **Usalo como complemento, nunca como unica fuente de aprendizaje.**

---

## Licencia

Este proyecto está licenciado bajo **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**.

[![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

Esto significa que puedes:
- **Compartir** — copiar y redistribuir el material en cualquier medio o formato
- **Adaptar** — remezclar, transformar y construir sobre el material para cualquier proposito, incluso comercial

Con las siguientes condiciones:
- **Atribucion** — Debes dar credito apropiado, proporcionar un enlace a la licencia e indicar si se realizaron cambios
- **CompartirIgual** — Si remezclas, transformas o creas a partir del material, debes distribuir tu contribucion bajo la misma licencia que el original

Ver el archivo [LICENSE](LICENSE) para más detalles.

---

## Homenaje a "El mundo de Beakman"

<p align="center">
  <a href="https://www.youtube.com/@ElMundodeBeakman-j2m/featured">
    <img src="https://img.shields.io/badge/YouTube-El%20Mundo%20de%20Beakman-red?style=for-the-badge&logo=youtube" alt="Canal de YouTube"/>
  </a>
</p>

Este proyecto es un humilde homenaje a **"El mundo de Beakman"** (*Beakman's World*), la serie de television educativa que entre 1992 y 1998 demostro que la ciencia podia ser divertida, accesible y emocionante.

Gracias a:

- **Paul Zaloom**, el actor que dio vida a Beakman con su energia inagotable, su pelo imposible y su capacidad unica para hacer que lo complejo pareciera sencillo.
- **Josie**, **Liza** y **Phoebe**, las asistentes que acompanaron a Beakman y demostraron que la curiosidad no tiene genero.
- **Lester**, la rata sarcastica que nos recordaba que hasta las preguntas mas "tontas" merecen una respuesta.
- **Jok Church**, creador del comic original "You Can with Beakman and Jax" que inspiro la serie.
- Todo el equipo de produccion que hizo posible que millones de ninos en todo el mundo descubrieran el placer de preguntar "¿por que?".

En una epoca sin internet ni YouTube, Beakman fue para muchos de nosotros la puerta de entrada al pensamiento cientifico. Su legado sigue vivo en cada profesor que explica con pasion, en cada padre que responde con paciencia, y en cada nino que no deja de preguntar.

> *"La ciencia no es dificil. Solo hay que explicarla bien."*

Este proyecto intenta mantener vivo ese espiritu: **aprender debe ser una aventura, no una obligacion**.

---

<p align="center">
  <em>"Entender es mas importante que memorizar"</em>
</p>

<p align="center">
  <em>"Entender es más importante que acertar"</em>
</p>
