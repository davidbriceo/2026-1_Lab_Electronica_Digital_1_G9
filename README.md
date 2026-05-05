# Laboratorio de Electrónica Digital I – G9  
**Semestre 2026-1**

Repositorio oficial del curso **Laboratorio de Electrónica Digital I**, asociado a la asignatura de Electrónica Digital I.  
Aquí se publicarán las guías, lineamientos, cronograma y material de apoyo para el desarrollo de las prácticas de laboratorio.

---

## 📌 Contenido
- [Introducción](#introducción)
- [Docente de laboratorio](#docente-de-laboratorio)
- [Metodología de trabajo](#metodología-de-trabajo)
- [Cronograma](#cronograma)
- [Entregables y documentación](#entregables-y-documentación)
- [Criterios de evaluación](#criterios-de-evaluación)
- [Normas generales del laboratorio](#normas-generales-del-laboratorio)
- [Herramientas de trabajo](#herramientas-de-trabajo)
- [Canales de comunicación](#canales-de-comunicación)

---

## Introducción

[Link préstamo en casa](https://docs.google.com/forms/d/e/1FAIpQLSfT5iicJ0mY-kWmhDDe7pbI3EFQC6DBiX97eUetKS784UjeYw/viewform)
[Link FPGA Colorlight](https://www.fervicom.com/producto/tarjeta-de-control-receptora-colorlight/?srsltid=AfmBOop5L2KnpznO7XTH_9p69gfeza_5DGTdJ6TIzAXGjiPXV8aQpcHj)

El **Laboratorio de Electrónica Digital I** es un espacio académico orientado a la **introducción al diseño de sistemas digitales**, en coherencia con los contenidos desarrollados en la asignatura magistral.

El laboratorio busca que el estudiante comprenda y aplique el **flujo básico de diseño digital**, partiendo de la especificación de un problema, pasando por su modelado y descripción en HDL, hasta su verificación mediante simulación.

A lo largo del curso, el estudiante trabajará con:
- **Lógica combinacional y secuencial**
- **Diseño modular y jerárquico**
- **Máquinas de estados finito (FSM)**
- **Introducción a máquinas de estado algorítmicas (ASM)**

Las prácticas están diseñadas para que el estudiante:
- Analice un problema a partir de sus **especificaciones funcionales**.
- Modele el sistema de forma estructurada (diagramas, FSM, ASM).
- Describa el comportamiento usando **HDL a nivel RTL**.
- Verifique el diseño mediante **simulación funcional**.
- Documente rigurosamente el proceso de diseño y sus resultados.

El laboratorio enfatiza el **aprendizaje progresivo**, el razonamiento ingenieril y la correcta articulación entre teoría y práctica, más allá de la simple escritura de código.

Adicionalmente, se utilizará **GitHub Classroom** como herramienta para control de versiones y documentación técnica, introduciendo al estudiante a prácticas habituales en entornos académicos y profesionales.

---

## Docente de laboratorio

**Docente:**  
*David Orlando Briceño González*  
Ingeniero Electrónico  
Correo institucional: *dbriceno@unal.edu.co*

**Grupos:**  
- Grupo G9 – *Martes de 9:00 a 11:00*  
---

## Metodología de trabajo

El laboratorio se desarrollará bajo una metodología **práctica, progresiva y estructurada**, orientada al aprendizaje activo.

### 1️⃣ Preparación previa
Antes de cada sesión, los estudiantes deberán:
- Revisar la **guía del laboratorio** correspondiente.
- Estudiar los conceptos teóricos necesarios.
- Verificar que su **entorno de trabajo** esté correctamente configurado.

### 2️⃣ Desarrollo en laboratorio
Durante la sesión:
- El docente realizará una **introducción conceptual breve**.
- Los estudiantes desarrollarán la práctica guiados por la metodología propuesta.
- Se fomentará el análisis, la discusión técnica y la justificación de decisiones de diseño.

### 3️⃣ Validación y análisis
Cada práctica deberá incluir:
- Simulación funcional del sistema diseñado.
- Comparación entre el comportamiento esperado y los resultados obtenidos.
- Identificación de errores, limitaciones y posibles mejoras.

---

## Cronograma

El cronograma de prácticas será publicado y actualizado en este repositorio.  
Cada laboratorio contará con su respectiva guía y fecha de entrega.

| Semana | Nombre                                   | Guía  | Entrega (GitHub Classroom) | Deadline |
|------|-------------------------------------------|-------|-----------------------------|----------|
| 1    | Lab 00 – Inducción y flujo de diseño digital | [lab00](https://github.com/davidbriceo/2026-1_Lab_Electronica_Digital_1_G9/tree/main/labs/lab00) | [Link](https://classroom.github.com/a/Yp_CVmX5)   | 17/02/2026      |
| 2    | Lab 01 – Sistemas Numéricos y Señales Digitales    | [lab01](https://github.com/davidbriceo/2026-1_Lab_Electronica_Digital_1_G9/tree/main/labs/lab01) | [Link](https://classroom.github.com/a/YpmfVGDw)                        | 25/04/2026      |
| 3    | Lab 02 – Compuertas Lógicas y Álgebra de Boole        | [lab02](https://github.com/davidbriceo/2026-1_Lab_Electronica_Digital_1_G9/tree/main/labs/lab02) | [Link](https://classroom.github.com/a/ajUf-Mh6)                        | 02/05/2026      |
| 4    | Lab 03 – Diseño modular y jerárquico / Diagramas de Flujo       | [lab03](https://github.com/davidbriceo/2026-1_Lab_Electronica_Digital_1_G9/tree/main/labs/lab03) | [Link](https://classroom.github.com/a/1cy-pJWy)                       |  09/05/2026     |
| 5    | Lab 04 – Lógica secuencial básica            | lab04 | Link                        | TBD      |
| 6    | Lab 05 – Máquinas de estados finito (FSM)   | lab05 | Link                        | TBD      |
| 7    | Lab 06 – FSM aplicadas                      | lab06 | Link                        | TBD      |
| 8    | Lab 07 – Introducción a ASM                 | lab07 | Link                        | TBD      |
| 9    | Lab 08 – Sistema secuencial basado en ASM   | lab08 | Link                        | TBD      |

---

## Entregables y documentación

- Cada práctica se documentará mediante un **informe técnico**.
- El informe se realizará en el archivo **`README.md`** del repositorio asignado por **GitHub Classroom**, utilizando **Markdown**.
- El repositorio podrá incluir:
  - Código HDL.
  - Diagramas (bloques, FSM, ASM).
  - Resultados de simulación.
  - Archivos adicionales solicitados en la guía.

El respeto por la estructura indicada en cada práctica es **obligatorio**.

---

## Criterios de evaluación

La evaluación del laboratorio se realizará con base en el **desarrollo de las prácticas**, la asistencia y la calidad del proceso de diseño y documentación.

---

### Rúbrica de evaluación de las prácticas

Cada práctica será evaluada con base en dos componentes:

#### 1️⃣ Demostración y explicación en laboratorio (40 %)
- Funcionamiento correcto del diseño.
- Capacidad de explicar el comportamiento del sistema.
- Coherencia entre especificación y resultados.
- Uso adecuado de las herramientas de simulación.

#### 2️⃣ Informe técnico y documentación (60 %)
- Descripción clara del problema y la solución.
- Diagramas y representaciones gráficas pertinentes.
- Resultados de simulación correctamente interpretados.
- Código organizado, legible y comentado.
- Uso adecuado de Markdown y estructura del repositorio.

---

## Normas generales del laboratorio

- La asistencia es obligatoria.
- Puntualidad y respeto por los tiempos asignados.
- Uso adecuado de los equipos e instalaciones.
- Mantener orden y limpieza en el laboratorio.
- Reportar cualquier falla o irregularidad.
- No se permite el consumo de alimentos.

---

## Herramientas de trabajo

### 💻 Sistema operativo
- Distribuciones Linux (Ubuntu, Linux Mint, u otras equivalentes). Si no maneja este sistema operativo y requiere un tutorial de cómo montarlo en paralelo con windows, le recomiendo visitar [este video](https://www.youtube.com/watch?v=wIj7sHK0SkQ), tenga cuidado y preste atención a las indicaciones dadas en la primera sesión

### 🛠️ Editor
- Visual Studio Code

### ⚙️ Diseño y simulación
- Icarus Verilog  
- GTKWave  

### 🌐 Control de versiones
- Git  
- GitHub / GitHub Classroom  

---

## Canales de comunicación

- **Correo institucional:** *dbriceno@unal.edu.co*  
- Anuncios oficiales a través de GitHub Classroom.

---


## Recursos adicionales:
- [Instalación de herramientas y plugins para la consola](src/custom_console.md)
- [Libro Fundamentos de Sistemas Digitales Floyd](https://drive.google.com/file/d/1G9gvkws5Ki07PLV2FFVLoGkdmUaq_tW7/view?usp=sharing)
- [Curso Verilog y FPGA en Youtube](https://www.youtube.com/watch?v=GLfnmc4Vv5U&list=PLIyIZGa1sAZqeQJ6Y02b7O8HV0gK25zc2)
- [Instalación Linux + Windows dualboot en el mismo disco](https://www.youtube.com/watch?v=wIj7sHK0SkQ)
- [Instalación Linux + Windows en discos diferentes, tenga mucho cuidado](https://www.youtube.com/watch?v=KWVte9WGxGE)
- [Curso en Coursera de verilog y HDL, primero debe solicitar el acceso al convenio al correo coursera@unal.edu.co](https://www.coursera.org/programs/coursera-para-la-universidad-nacional-de-colombia-ji3sj/learn/fpga-hardware-description-languages?source=search#modules)
