# CLAUDE.md

Este archivo proporciona orientación a Claude Code (claude.ai/code) para trabajar con este repositorio.

## Descripción del Proyecto

Este repositorio contiene la base de conocimiento y el prompt del sistema para un GPT personalizado llamado "Beakman" - un tutor de matemáticas creado para ayudar a una estudiante de 1º de la ESO a aprender matemáticas.

## Configuración del GPT (GPT Builder)

**Nombre:** Mi mundo de Beakman (MATEMATICAS)

**Descripción:** Guía interactiva para enseñar y explorar Matemáticas. Inspirado en el estilo de Beakman: curioso, divertido y reflexivo. Diseñado para profesores, familias y uso educativo supervisado.

**Iniciadores de conversación:**
- 🧭 ¿Te has quedado en blanco o no sabes por dónde empezar? Escribe Ayuda y te guío paso a paso.
- 📚 Quiero repasar un tema
- ❓ No entiendo este ejercicio (pega o describe el ejercicio)
- 🎯 Dame un ejercicio para practicar

**Imagen:** `gpt/logo.jpeg`

**Instrucciones:** Contenido de `gpt/Curso_Matematicas_1ESO_Prompt.txt`

**Knowledge (archivos a subir):** Todo el contenido de la carpeta `knowledge/`

## Estructura del Repositorio

```
/beakman_math
├── CLAUDE.md
├── gpt/                    # Configuración del GPT
│   ├── logo.jpeg           # Imagen del GPT
│   └── Curso_Matematicas_1ESO_Prompt.txt  # Instrucciones
├── knowledge/              # Archivos de Knowledge (subir al GPT)
│   ├── 00_Mapa_del_Curso_Matematicas.txt
│   ├── 01_Numeros_Naturales.txt
│   ├── 02_Divisibilidad.txt
│   ├── ...
│   └── 10_Estadistica_y_Probabilidad.txt
└── docs/                   # Documentación interna
    └── Curso_Matematicas_1ESO_Prompt_Comentado.txt
```

## Temas del Currículo (Orden Progresivo)

1. Números Naturales
2. Divisibilidad
3. Fracciones
4. Decimales
5. Fracciones y Decimales
6. Porcentajes
7. Álgebra Inicial
8. Medida
9. Geometría Plana
10. Estadística y Probabilidad

## Filosofía Pedagógica de Beakman

El asistente prioriza:
- **Comprensión sobre memorización** - entender el porqué, no solo el cómo
- **Explicaciones visuales primero** - imágenes mentales → palabras → símbolos matemáticos
- **Conexión con la vida real** - relacionar las matemáticas con situaciones cotidianas
- **El error como aprendizaje** - los errores son parte del proceso, nunca se ridiculizan

Estructura estándar de explicación:
1. Introducción visual
2. Idea matemática central
3. Ejemplo cotidiano
4. Preguntas para pensar
5. Mini comprobación
6. Opciones para continuar

## Trabajar con Este Repositorio

Al editar los archivos de temas, mantener el formato consistente:
- Título del tema
- Descripción breve
- "Ideas clave"
- "Errores típicos"
- "Relación con otros temas"

Todo el contenido debe ser apropiado para estudiantes de 12 años.
