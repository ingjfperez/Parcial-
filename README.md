# Parcial-
Insumos 

# Parcialito-seg-corte
insumos para el parcial de POO2026-1


# PARCIAL DE PROGRAMACIÓN ORIENTADA A OBJETOS (POO)

## Plataforma Digital de Contenidos (Streaming & Learning)

**Duración:** 1.5 horas  
**Modalidad:** Individual o en parejas (máximo 2 estudiantes)  
**Lenguaje:** Java  

---

## 1. Objetivo

Evaluar la capacidad del estudiante para diseñar soluciones utilizando los principios fundamentales de la Programación Orientada a Objetos (POO), específicamente:

- Abstracción
- Encapsulamiento
- Herencia
- Polimorfismo (incluyendo sobrecarga de métodos)
- Interfaces
- Principio SOLID: Responsabilidad Única (SRP)

---

## 2. Contexto del Problema

Una startup tecnológica inspirada en plataformas como Netflix, Spotify y Coursera requiere desarrollar un sistema base para la gestión de contenidos digitales.

La plataforma permitirá administrar diferentes tipos de contenido, tales como:

- Películas
- Canciones
- Cursos

Cada tipo de contenido comparte características comunes, pero también presenta comportamientos específicos. Adicionalmente, algunos contenidos permiten el seguimiento del progreso del usuario.

El sistema debe diseñarse aplicando buenas prácticas de POO, garantizando modularidad, escalabilidad y mantenibilidad.

---

## 3. Requerimientos del Sistema

### 3.1 Abstracción y Encapsulamiento (30%)

1. Crear una clase abstracta denominada `ContenidoDigital` que incluya:

   **Atributos privados:**
   - `titulo`
   - `duracion` (en minutos)

   **Métodos:**
   - `reproducir()` (abstracto)
   - `pausar()` (abstracto)
   - `mostrarInformacion()` (concreto)

2. Implementar encapsulamiento mediante:
   - Métodos getters y setters
   - Validaciones:
     - La duración no puede ser negativa
     - El título no puede estar vacío

---

### 3.2 Herencia e Interfaces (25%)

1. Crear una interfaz `Progreso` con el método:
   - `marcarProgreso(int porcentaje)`

2. Crear las siguientes clases:
   - `Pelicula`
   - `Cancion`
   - `Curso`

3. Condiciones:
   - Todas las clases deben heredar de `ContenidoDigital`
   - La clase `Curso` debe implementar la interfaz `Progreso`
   - Cada clase debe implementar sus propios métodos:
     - `reproducir()`
     - `pausar()`

---

### 3.3 Polimorfismo y Sobrecarga (20%)

1. Implementar sobrecarga del método `reproducir`:
   - `reproducir()`
   - `reproducir(int minutoInicio)`

2. Demostrar polimorfismo:
   - Crear una colección (`ArrayList`)opcional de tipo `ContenidoDigital`
   - Almacenar diferentes tipos de contenidos
   - Recorrer la colección y ejecutar los métodos correspondientes

---

### 3.4 Principio SOLID: Responsabilidad Única (15%)

1. Crear una clase denominada `PlataformaStreaming` cuya responsabilidad sea:

   - Registrar contenidos
   - Listar contenidos
   - Mostrar información de los contenidos

2. Restricción:
   - No incluir lógica de negocio en la clase `Main`
   - Cada clase debe tener una única responsabilidad claramente definida

---

### 3.5 Programa Principal (10%)

1. Crear una clase `Main` que:

   - Instancie diferentes tipos de contenido
   - Utilice la clase `PlataformaStreaming`
   - Ejecute:
     - Métodos de reproducción
     - Métodos de pausa
     - Visualización de información
     - Seguimiento de progreso (cuando aplique)

---

## 4. Restricciones Generales

- No se permite el uso de atributos públicos
- No se permite la duplicación de lógica entre clases
- Los nombres de métodos deben ser claros y descriptivos
- Se debe respetar el principio de responsabilidad única (SRP)
- Se debe mantener una adecuada organización del código

---

## 5. Criterios de Evaluación

| Criterio                                      | Puntos |
|----------------------------------------------|--------|
| Implementación de clase abstracta            | 10     |
| Encapsulamiento y validaciones              | 10     |
| Uso adecuado de herencia                    | 10     |
| Implementación de interfaces                | 10     |
| Sobrecarga de métodos                      | 10     |
| Polimorfismo funcional                     | 10     |
| Aplicación del principio SRP                | 15     |
| Organización y claridad del código          | 10     |
| Funcionamiento del sistema                 | 15     |
| **Total**                                   | **100**|

Se debe realizar una regla de 3 para saber su nota sobre 15 puntos

---

## 6. Bonificación (Opcional +10 puntos)

- Uso de `ArrayList` de forma adecuada
- Implementación de validaciones adicionales
- Personalización de mensajes según el tipo de contenido
- Código limpio y bien estructurado

---

## 7. Observaciones

- La concentración de lógica en la clase `Main` será penalizada
- La ausencia de polimorfismo implica la pérdida del puntaje correspondiente
- La duplicación de código afecta negativamente la evaluación
- El uso de nombres genéricos o poco descriptivos impacta la calificación
- Se evaluará tanto la funcionalidad como la calidad del diseño

---

## 8. Entregables

El estudiante debe entregar:

- Código fuente completo en Java
- Proyecto compilable y ejecutable
- Estructura organizada en paquetes (si aplica)

---

## 9. Recomendaciones

- Planificar antes de codificar
- Identificar claramente las responsabilidades de cada clase
- Aplicar buenas prácticas de programación
- Validar el funcionamiento antes de la entrega

---



