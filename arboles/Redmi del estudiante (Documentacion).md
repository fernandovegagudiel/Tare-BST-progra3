# Implementación de Operaciones sobre un Árbol Binario de Búsqueda

## Contexto

El proyecto consiste en la construcción de un Árbol Binario de Búsqueda (BST) utilizando Java. Sobre esta estructura se desarrollaron diferentes algoritmos enfocados en análisis, validación y transformación del árbol.

La implementación fue realizada mediante nodos enlazados y recorridos recursivos, permitiendo manipular la estructura sin utilizar librerías externas especializadas.

---

# Herramientas utilizadas

| Recurso | Utilización |
|----------|------------|
| Java 17 | Desarrollo del proyecto |
| Maven | Compilación |
| Eclipse | Edición y pruebas |
| Git | Control de versiones |
| GitHub | Respaldo del código |

---

# Ejecución

## Compilar

```bash
mvn clean compile
```

## Ejecutar

```bash
mvn exec:java -Dexec.mainClass="umg.edu.progra.arboles.Principal"
```

---

# Funcionalidades desarrolladas

## Conteo recursivo de elementos

### Finalidad

Obtener la cantidad real de nodos existentes en la estructura.

### Implementación

El algoritmo visita cada nodo exactamente una vez y acumula el total mediante llamadas recursivas.

### Resultado observado

```text
Cantidad total: 8
```

---

## Análisis de balance

### Finalidad

Determinar si la distribución de nodos mantiene una diferencia aceptable entre ramas.

### Implementación

Para cada nodo se calculan las alturas de sus subárboles y se verifica que la diferencia sea mínima.

### Resultados

```text
Árbol principal: balanceado
```

```text
Árbol de prueba: no balanceado
```

---

## Verificación estructural

### Finalidad

Comprobar que la organización interna continúa respetando las reglas de un BST.

### Implementación

Se utilizan límites mínimos y máximos durante el recorrido para validar cada posición.

### Resultados

```text
BST válido
```

```text
BST inválido
```

---

## Ancestro compartido

### Finalidad

Encontrar el nodo común más cercano entre dos valores determinados.

### Casos ejecutados

| Valores | Resultado |
|----------|-----------|
| 10 y 40 | 30 |
| 10 y 80 | 50 |
| 60 y 80 | 70 |

---

## Conversión espejo

### Finalidad

Modificar la estructura para generar una representación invertida.

### Resultado

Antes:

```text
10 20 30 40 50 60 70 80
```

Después:

```text
80 70 60 50 40 30 20 10
```

---

# Funciones complementarias

## Búsqueda por posición ordenada

Permite identificar el elemento que ocupa una posición específica dentro de la secuencia ordenada del árbol.

### Ejemplos

```text
Posición 1 -> 10
Posición 3 -> 30
Posición 5 -> 50
Posición 8 -> 80
```

---

## Consulta por intervalo

Recupera únicamente los elementos que pertenecen a un rango definido.

### Ejemplo

```text
Rango solicitado:
20 - 60

Resultado:
20 30 40 50 60
```

---

## Cálculo del diámetro

Obtiene la longitud del recorrido más extenso posible entre dos nodos.

### Resultado

```text
Diámetro = 5
```

---

## Creación dinámica desde parámetros

El programa admite la recepción de valores desde la línea de ejecución para construir automáticamente un BST.

### Parámetros utilizados

```text
40 18 65 8 25 55 90
```

### Salida obtenida

```text
8 18 25 40 55 65 90
```

---

# Resultados generales

La práctica permitió implementar y validar múltiples algoritmos relacionados con árboles binarios de búsqueda, reforzando conocimientos de:

- Recursividad.
- Estructuras jerárquicas.
- Recorridos de árboles.
- Validación de propiedades BST.
- Manipulación de nodos.
- Gestión de versiones mediante Git.

El resultado final es una implementación funcional capaz de resolver tanto operaciones básicas como problemas de análisis estructural sobre árboles binarios.
