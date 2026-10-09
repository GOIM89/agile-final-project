---
name: Historia de usuario
about: Plantilla para describir una necesidad funcional con criterios de aceptación verificables
---

## Historia de usuario

Completa cada frase con un rol específico, una capacidad concreta y el beneficio esperado.

**Como** [rol específico, por ejemplo: cliente, administrador del catálogo o desarrollador]

**Necesito** [acción o capacidad que el sistema debe ofrecer]

**Para que** [beneficio que obtendrá el usuario o el negocio]

## Criterios de aceptación

Escribe uno o más escenarios. En cada escenario, describe el contexto en **Dado**, la acción en **Cuando** y un resultado observable en **Entonces**.

### Escenario: [nombre del resultado esperado]

- **Dado** [contexto inicial y datos necesarios]
- **Cuando** [acción que realiza el usuario]
- **Entonces** [resultado observable y verificable]

### Escenario alternativo: [error o condición límite]

- **Dado** [contexto alternativo]
- **Cuando** [acción que realiza el usuario]
- **Entonces** [respuesta esperada del sistema]

## Ejemplo completo: crear un producto

**Como** administradora del catálogo

**Necesito** registrar un producto con nombre, descripción y precio

**Para que** los clientes puedan encontrarlo y conocer su precio antes de comprar.

### Escenario: crear un producto con datos válidos

- **Dado** que la administradora inició sesión y proporciona nombre, descripción y precio mayor que cero
- **Cuando** guarda el producto
- **Entonces** el sistema lo registra y lo muestra en el catálogo con esos datos

### Escenario: rechazar un precio no válido

- **Dado** que la administradora proporciona un precio igual o menor que cero
- **Cuando** intenta guardar el producto
- **Entonces** el sistema muestra un mensaje de validación y no registra el producto

### Escenario: solicitar los datos obligatorios

- **Dado** que falta el nombre o la descripción del producto
- **Cuando** la administradora intenta guardarlo
- **Entonces** el sistema indica qué dato falta y no registra el producto
