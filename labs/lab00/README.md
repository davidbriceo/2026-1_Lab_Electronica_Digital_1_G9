# Lab00: Inducción al Laboratorio y Flujo de Diseño Digital

## Contenido
- Objetivos de aprendizaje  
- Fundamento teórico  
- Procedimiento  
- Descripción del HDL base  
- Entregables  

---

## 1. Objetivos de aprendizaje

Al finalizar esta práctica, el estudiante será capaz de:

- Comprender el **rol del Laboratorio de Electrónica Digital I** dentro de la línea curricular.
- Identificar el **flujo básico de diseño digital** desde la especificación hasta la simulación.
- Reconocer la diferencia entre **problema, arquitectura y código**.
- Configurar y verificar un entorno básico de trabajo en **Linux** para diseño digital.
- Compilar y simular **módulos combinacionales simples en Verilog**.
- Visualizar señales digitales mediante **GTKWave**.

---

## 2. Fundamento teórico

### 2.1 ¿Qué significa “hacer diseño digital”?

El diseño digital no consiste únicamente en escribir código HDL.  
Un sistema digital se desarrolla siguiendo un **proceso estructurado**, que incluye:

1. **Especificación del problema**  
   Qué debe hacer el sistema.
2. **Arquitectura de solución**  
   Cómo se organiza el sistema (bloques, señales, jerarquía).
3. **Descripción en HDL**  
   Implementación del comportamiento en Verilog.
4. **Verificación**  
   Comprobación del funcionamiento mediante simulación.
5. **Análisis de resultados**  
   Validación frente a lo esperado.

Este laboratorio introduce este flujo de trabajo desde la primera práctica.

---

### 2.2 Lógica combinacional y lógica secuencial

En **lógica combinacional**, las salidas dependen únicamente de las entradas actuales.  
No existe memoria ni dependencia del tiempo.

En **lógica secuencial**, el sistema incorpora memoria y su comportamiento depende:
- del estado previo,
- de las entradas,
- y del reloj.

En este laboratorio inicial se trabajará **exclusivamente con lógica combinacional**, preparando el terreno para la lógica secuencial en prácticas posteriores.

---

### 2.3 Importancia de la simulación

La simulación es una herramienta fundamental en el diseño digital, ya que permite:

- Verificar el comportamiento del sistema antes de su implementación.
- Detectar errores de diseño de manera temprana.
- Analizar señales internas que no siempre son visibles en hardware.

En este curso, **todo diseño debe ser simulado** antes de considerarse correcto.

---

## 3. Procedimiento

### 3.0 Instalación del entorno de trabajo

Antes de iniciar los ejercicios del laboratorio, es necesario contar con un entorno básico para el desarrollo y simulación en Verilog.  
Se utilizarán herramientas **open source**:

- **Icarus Verilog**: compilador y simulador de Verilog HDL.
- **GTKWave**: visualizador de formas de onda.
- Un editor de código fuente (por ejemplo, VS Code).

#### Icarus-Verilog es un compilador *open source* para Verilog HDL.

Actualice la lista de paquetes de Linux, luego instale Icarus Verilog como se muestra:

```
sudo apt update
```

```
sudo apt install iverilog
```

Para comprobar la instalación basta con ejecutar el siguiente comando para verificar la versión instalada:

```
iverilog -v
```


##### Instalación de GTKWave

GTKWave es un visor de formas de onda que funciona con Icarus Verilog para mostrar los resultados de la simulación. Está convenientemente disponible en la lista de paquetes apt de Ubuntu, por lo tanto es posible usar el comando ```apt install``` de nuevo:


```
sudo apt install gtkwave
```

Para verificar la instalación basta con ejecutar el comando ```gtkwave``` en la terminal y deberá ejecutarse el programa.



### 3.0 Verificación del entorno de trabajo (Smoke Test: si lo enciendo y no sale humo, al menos algo básico funciona)

1. Compile y simule un módulo combinacional simple en Verilog.
2. Genere un archivo `.vcd`.
3. Visualice las señales en GTKWave para verificar el correcto funcionamiento del entorno.

Paso a paso: 
Descargue el archivo [smoke_andor.v](src/smoke_andor.v) y el archivo [tb_smoke_andor.v](src/tb_smoke_andor.v) y visualícelos.

Ejecute los siguientes comandos:
1. Compilar (-o)
`iverilog -o tb_smoke_andor.vvp tb_smoke_andor.v`
2. Simular (vvp = generar el .vcd)
`vvp tb_smoke_andor.vvp`
3. Ver ondas en GTKWave
`gtkwave`
New tab, abrir el archivo .vcd, poner las señales de su interés:

![Resultado del smoke test en GTKWave](src/imgs/lab00_demo_gtkwave.png)

---

### 3.2 Ejercicio 1 (Grupal): Análisis de un sistema digital

#### Descripción
Seleccione un sistema digital cotidiano (por ejemplo: semáforo, contador, cerradura digital, temporizador) y realice su **análisis funcional**, sin implementar aún lógica secuencial.

#### Actividades
- Identificar:
  - Entradas.
  - Salidas.
- Describir el comportamiento del sistema en lenguaje natural.
- Proponer un **diagrama de caja negra**.

Este ejercicio **no requiere código HDL**.

---

### 3.3 Ejercicio 2 (Grupal): Implementación combinacional básica

#### Descripción
Diseñar e implementar en Verilog un **módulo combinacional simple**, de acuerdo con una especificación dada por el docente.

Ejemplos posibles:
- Comparador.
- Codificador / decodificador.
- Lógica de control simple.

#### Requisitos
- Describir el módulo en Verilog.
- Implementar un **testbench**.
- Verificar el funcionamiento mediante simulación.

---

## 4. Descripción del HDL base

Para los módulos combinacionales implementados se debe considerar:

- Uso adecuado de `assign` o bloques `always @(*)`.
- Definición clara de entradas y salidas.
- Código legible y organizado.
- Separación entre **módulo de diseño** y **testbench**.

El testbench debe incluir:
- Estímulos representativos.
- Generación del archivo `.vcd`.
- Comentarios que expliquen los casos de prueba.

---

## 5. Entregables

- Documentación del laboratorio en el archivo `README.md`.
- Carpeta `src/` con:
  - Código Verilog del módulo combinacional.
  - Testbench correspondiente.
- Evidencias de simulación (capturas de GTKWave).
- Diagrama de caja negra del sistema analizado.
- Demostración básica del funcionamiento durante la sesión de laboratorio.

Todos los archivos deben cargarse en el repositorio asignado en **GitHub Classroom**.

---

## Recursos adicionales
- [Introducción a Verilog HDL](https://www.youtube.com/watch?v=GLfnmc4Vv5U)
- [Uso básico de GTKWave](https://www.youtube.com/watch?v=0WZzq8kD8qY)
