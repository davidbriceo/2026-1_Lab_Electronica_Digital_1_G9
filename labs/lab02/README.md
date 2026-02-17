# Lab02: Compuertas Lógicas y Álgebra de Boole

## Contenido
- Objetivos de aprendizaje  
- Fundamento teórico  
- Procedimiento  
- Descripción del enfoque lógico  
- Entregables  

---

## 1. Objetivos de aprendizaje

Al finalizar esta práctica, el estudiante será capaz de:

- Identificar y representar compuertas lógicas básicas.
- Construir tablas de verdad.
- Traducir un problema físico a una expresión booleana.
- Aplicar leyes del álgebra de Boole.
- Aplicar el teorema de De Morgan.
- Simplificar funciones lógicas.
- Diseñar circuitos combinacionales a nivel simbólico.

---

## 2. Fundamento teórico

### 2.1 Compuertas lógicas básicas

- AND (Producto)
- OR (Suma)
- NOT (Complemento)
- NAND
- NOR
- XOR

Cada compuerta puede representarse mediante:

- Símbolo gráfico (IEEE/ANSI)
- Tabla de verdad
- Expresión booleana

---

### 2.2 Álgebra de Boole

Operaciones fundamentales:

- Negación: X’
- Producto: X·Y
- Suma: X + Y

Leyes importantes:

- Conmutativa
- Asociativa
- Distributiva
- Identidad
- Complemento
- Absorción

---

### 2.3 Teorema de De Morgan

(X + Y)’ = X’ · Y’  
(X · Y)’ = X’ + Y’

Estos teoremas permiten transformar circuitos con NAND y NOR.

---

## 3. Procedimiento

### 3.1 Parte A – Tablas de verdad

Construya las tablas de verdad de:

1. NAND
2. NOR
3. XOR
4. Función: X = (A + B’) · C

---

### 3.2 Parte B – Simplificación algebraica

Simplifique paso a paso:

1. X = A + A·B
2. X = (A + B)(A + C)
3. X = A·B + A·B’
4. X = (A + B)’ + A·B

Justifique cada paso indicando la ley utilizada.

---

### 3.3 Parte C – Aplicación del Teorema de De Morgan

Aplique De Morgan y simplifique:

1. (A + B + C)’
2. (A·B·C)’
3. (A + B)’ · (A + C)’

---

### 3.4 Parte D – Ejercicio Floyd (Tren de aterrizaje)

Se requiere un circuito para indicar el estado del tren de aterrizaje:

- LED verde se enciende si los tres mecanismos están extendidos.
- LED rojo se enciende si alguno falla.
- Cuando el mecanismo está extendido → sensor = 0.
- Cuando está retraído → sensor = 1.

#### Actividades

1. Definir variables:
   - A, B, C (sensores)
   - S (switch bajar tren)
   - V (LED verde)
   - R (LED rojo)

2. Construir la tabla de verdad.
3. Obtener la expresión booleana de:
   - LED verde
   - LED rojo
4. Simplificar.
5. Dibujar el circuito lógico.

---

## 4. Descripción del enfoque lógico

En esta práctica no se utilizará HDL.

Se trabajará exclusivamente en:

- Representación algebraica.
- Tablas de verdad.
- Diagramas de compuertas.
- Simplificación formal.

Esta práctica prepara la transición hacia la implementación en Verilog en el siguiente laboratorio.

---

## 5. Entregables

El README.md debe incluir:

- Tablas de verdad completas.
- Procedimiento de simplificación paso a paso.
- Aplicación detallada de De Morgan.
- Solución completa del ejercicio Floyd:
  - Tabla de verdad
  - Expresión final
  - Circuito dibujado
- Explicación breve (máximo 5 líneas):
  ¿Por qué NAND y NOR se consideran compuertas universales?

---
