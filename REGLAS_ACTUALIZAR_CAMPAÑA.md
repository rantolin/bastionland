# Reglas para la Actualización del Vault de Mythic Bastionland

Este documento define el conjunto de reglas y procedimientos que se deben seguir para actualizar el vault de Obsidian después de transcribir una nueva nota de sesión (`Sesion-N.md`). El objetivo es mantener la coherencia y la interconexión de la información de la campaña.

## Workflow General Post-Sesión

El proceso se activa siempre que se crea o modifica una nota de sesión.

1.  **Lectura de la Sesión:** Analizar el contenido completo del archivo `Sesiones/Sesion-N.md` recién creado.
2.  **Identificación de Entidades:** Buscar todas las menciones de entidades existentes o nuevas que correspondan a las siguientes categorías:
    *   `@PNJs`
    *   `@Personajes` (PCs)
    *   `@Lugares`
    *   `@Caballeros` (personajes del lore)
3.  **Ejecución de Reglas:** Aplicar las reglas específicas para cada categoría, distinguiendo entre la actualización de una nota existente y la creación de una nueva.

---

## 1. Reglas para `@PNJs`

### 1.1. Actualización de Notas de PNJ Existentes

**Objetivo:** Añadir un resumen de la interacción con un PNJ ya conocido.

**Procedimiento:**

1.  En `Sesion-N.md`, localizar una mención a un PNJ existente (p. ej., `[[Bohumir]]`).
2.  Abrir el archivo correspondiente: `PNJs/Bohumir.md`.
3.  Navegar a la sección `# Apariciones e Interacciones`.
4.  Añadir una nueva línea con un enlace a la sesión actual y un resumen de lo ocurrido.

**Ejemplo:**
Si en `Sesion-6.md` los personajes vuelven a hablar con Bohumir y este les cuenta un nuevo rumor.

*   **Archivo a modificar:** `PNJs/Bohumir.md`
*   **Contenido a añadir bajo `# Apariciones e Interacciones`:**
    ```markdown
    *   **[[Sesion-6]]**: La compañía lo encuentra de nuevo en un cruce de caminos. Les habla sobre un extraño caballero que vio cerca del río y les vende una poción de curación menor.
    ```

### 1.2. Creación de Nuevas Notas de PNJ

**Objetivo:** Crear una ficha para un PNJ que aparece por primera vez y enlazarla desde la sesión.

**Procedimiento:**

1.  En `Sesion-N.md`, identificar un nuevo PNJ que no tiene nota (p. ej., "conocen a Elara, la herrera del pueblo").
2.  Crear un nuevo archivo en `PNJs/Elara, la herrera.md`.
3.  Rellenar el archivo usando la plantilla de abajo.
4.  **Volver a `Sesion-N.md` y reemplazar el texto "Elara, la herrera" por un enlace: `[[Elara, la herrera]]`.**

**Plantilla para nuevo PNJ:**
```markdown
# Quién es
[Breve descripción del PNJ basada en la información de la sesión. Quién es, a qué se dedica, cómo es su personalidad, etc.]

# Apariciones e Interacciones
*   **[[Sesion-N]]**: [Resumen del primer encuentro. Dónde estaba, qué hizo, qué información dio, etc.]
```

---

## 2. Reglas para `@Personajes` (PCs)

### 2.1. Actualización de Notas de Personaje

**Objetivo:** Registrar las acciones notables de los personajes jugadores en la sesión.

**Procedimiento:**

1.  En `Sesion-N.md`, identificar las acciones clave realizadas por cada personaje jugador (p. ej., `[[Ser Morcant the Gloomy (Chain Knight)]]`).
2.  Abrir el archivo del personaje: `Personajes/Ser Morcant the Gloomy (Chain Knight).md`.
3.  Navegar a la sección `# Acciones Notables`.
4.  Añadir un nuevo encabezado para la sesión actual y un listado con las acciones más importantes. Si el encabezado de la sesión ya existe, añadir las acciones a la lista.

**Ejemplo:**
Si en `Sesion-6.md`, Ser Morcant descifra un acertijo y derrota a un enemigo importante.

*   **Archivo a modificar:** `Personajes/Ser Morcant the Gloomy (Chain Knight).md`
*   **Contenido a añadir bajo `# Acciones Notables`:**
    ```markdown
    *   **[[Sesion-6]]**:
        *   Descifró el acertijo de la puerta de piedra, permitiendo el paso al grupo.
        *   Derrotó en combate singular al capitán de los bandidos.
    ```

### 2.2. Enlazado de Menciones de Personajes

**Objetivo:** Asegurar que todas las menciones a personajes existentes en una nota de sesión estén correctamente enlazadas a su ficha de personaje.

**Procedimiento:**

1.  En `Sesion-N.md`, leer el texto y buscar nombres o apodos de los personajes jugadores que no estén dentro de un enlace `[[...]]`. (p. ej., el texto plano "Ser Morcant").
2.  Conocer la lista de Personajes Jugarores y sus archivos correspondientes (p. ej., `Ser Morcant the Gloomy (Chain Knight).md`).
3.  Reemplazar el texto plano con el enlace correcto, usando un alias si es necesario para mantener la fluidez del texto.

**Ejemplo:**
Si en `Sesion-7.md` se escribe la frase: "Al día siguiente, Ser Morcant decidió explorar el bosque."

*   **Archivo a modificar:** `Sesion-7.md`
*   **Texto original:** `...Ser Morcant decidió explorar...`
*   **Texto modificado:** `...[[Ser Morcant the Gloomy (Chain Knight)|Ser Morcant]] decidió explorar...`

---

## 3. Reglas para `@Lugares`

### 3.1. Actualización de Notas de Lugar Existentes

**Objetivo:** Registrar los eventos que ocurren en un lugar ya conocido.

**Procedimiento:**

1.  En `Sesion-N.md`, localizar una mención a un lugar existente (p. ej., `[[Castillo de Cosnice]]`) donde ocurra algo.
2.  Abrir el archivo correspondiente: `Lugares/Castillo de Cosnice.md`.
3.  Navegar a la sección `# Sucesos Notables` (o similar, como `# Visitas y Sucesos`).
4.  Añadir una nueva línea describiendo el evento y enlazando la sesión.

**Ejemplo:**
Si en `Sesion-6.md` la compañía llega por fin al Castillo de Cosnice.

*   **Archivo a modificar:** `Lugares/Castillo de Cosnice.md`
*   **Contenido a añadir bajo `# Sucesos Notables`:**
    ```markdown
    *   **Llegada de la compañía ([[Sesion-6]]):** El grupo de caballeros es recibido en el castillo por [[Ser Howel, The Bone Knight]]. Se celebra un banquete en su honor.
    ```

### 3.2. Creación de Nuevas Notas de Lugar

**Objetivo:** Crear una ficha para un lugar descubierto por primera vez y enlazarla desde la sesión.

**Procedimiento:**

1.  En `Sesion-N.md`, identificar un nuevo lugar importante (p. ej., "descubren la Torre del Viento").
2.  Crear un nuevo archivo en `Lugares/Torre del Viento.md`.
3.  Rellenar el archivo usando la plantilla de abajo.
4.  **Volver a `Sesion-N.md` y reemplazar el texto "la Torre del Viento" por un enlace: `[[Torre del Viento]]`.**


**Plantilla para nuevo Lugar:**
```markdown
# Descripción
[Descripción del lugar basada en lo narrado en la sesión. Apariencia, atmósfera, detalles importantes.]

# Sucesos Notables
*   **Descubrimiento ([[Sesion-N]]):** [Resumen de cómo y cuándo la compañía encontró el lugar, y qué ocurrió durante la primera visita.]
```

---

## 4. Reglas para `@Caballeros` (Lore)

### 4.1. Actualización de Notas de Caballero Existente

**Objetivo:** Registrar nueva información o menciones sobre caballeros legendarios o importantes del lore.

**Procedimiento:**

1.  En `Sesion-N.md`, localizar una mención a un caballero del lore (p. ej., `[[The Dusk Knight]]`).
2.  Abrir el archivo correspondiente: `Caballeros/The Dusk Knight.md`.
3.  Si se revela nueva información sobre él, añadirla en la sección `# Información Conocida`.
4.  Añadir una nueva línea en la sección `# Apariciones y Menciones` para registrar dónde y cómo fue mencionado.

**Ejemplo:**
Si en `Sesion-6.md` un anciano cuenta que The Dusk Knight fue quien forjó una espada legendaria.

*   **Archivo a modificar:** `Caballeros/The Dusk Knight.md`
*   **Contenido a añadir en `# Información Conocida`:**
    ```markdown
    *   Según una leyenda local, fue el herrero original de la espada legendaria *Caminante del Ocaso*.
    ```
*   **Contenido a añadir en `# Apariciones y Menciones`:**
    ```markdown
    *   **[[Sesion-6]]**: Mencionado en una leyenda contada por un anciano en la aldea de Puentepiedra.
    ```

### 4.2. Creación de Nuevas Notas de Caballero

**Objetivo:** Crear una ficha para un caballero del lore mencionado por primera vez y enlazarla desde la sesión.

**Procedimiento:**

1.  En `Sesion-N.md`, identificar a un nuevo caballero del lore (p. ej., "la leyenda de 'La Dama de Hierro'").
2.  Crear un nuevo archivo: `Caballeros/La Dama de Hierro.md`.
3.  Rellenar el archivo con la plantilla de abajo.
4.  **Volver a `Sesion-N.md` y reemplazar el texto "La Dama de Hierro" por un enlace: `[[La Dama de Hierro]]`.**

**Plantilla para nuevo Caballero:**
```markdown
# Información Conocida
[Resumen de la leyenda o los datos que se han contado sobre este caballero en la sesión.]

# Apariciones y Menciones
*   **[[Sesion-N]]**: [Contexto de cómo fue mencionado por primera vez.]
```

---

## 5. Reglas para `@Mitos`

**Objetivo:** Registrar y seguir la evolución de los mitos, desde rumores hasta realidades, que es una mecánica central de Mythic Bastionland.

### 5.1. Creación de Nuevas Notas de Mito

**Objetivo:** Crear una ficha para un nuevo mito y enlazarlo desde la sesión.

**Procedimiento:**

1.  En `Sesion-N.md`, identificar un nuevo rumor, leyenda o suceso extraño que pueda convertirse en un mito (p. ej., las "cigüeñas llevando cadáveres").
2.  Crear un nuevo archivo en la carpeta `Mitos/`, con un nombre descriptivo (p. ej., `Mitos/Cigueñas Carroñeras.md`).
3.  Rellenar el archivo usando la plantilla de abajo.
4.  **Volver a `Sesion-N.md` y reemplazar el texto relevante (p. ej., "cigüeñas carroñeras") por un enlace: `[[Cigueñas Carroñeras]]`.**

**Plantilla para nuevo Mito:**
```markdown
# Descripción del Mito
[Resumen del mito tal y como se conoce hasta ahora.]

## Augurios (0/6)
*   **1er Augurio:** [Descripción del primer augurio o evento que inicia el mito, con enlace a la sesión donde ocurrió.]

# Historial de Avances
*   **[[Sesion-N]]**: [Contexto de cómo se originó el mito o se escuchó el primer rumor.]
```

### 5.2. Actualización de Notas de Mito Existentes

**Procedimiento:**

1.  En `Sesion-N.md`, identificar un suceso que pueda interpretarse como un nuevo augurio para un mito existente.
2.  Abrir el archivo del mito correspondiente (p. ej., `Mitos/Cigueñas Carroñeras.md`).
3.  Actualizar el contador de Augurios en el encabezado.
4.  Añadir el nuevo augurio a la lista de `## Augurios`.
5.  Añadir una entrada en el `# Historial de Avances` para registrar el evento de la sesión actual.

**Ejemplo:**
Si en `Sesion-7.md` los jugadores encuentran un nido gigante lleno de restos de armaduras.

*   **Archivo a modificar:** `Mitos/Cigueñas Carroñeras.md`
*   **Contenido a modificar/añadir:**
    ```markdown
    ## Augurios (2/6)
    *   **1er Augurio:** Una bandada de cigüeñas carroñeras es vista transportando los cadáveres de un caballero y su escudero envueltos en telarañas ([[Sesion-5]]).
    *   **2do Augurio:** Se descubre un nido de cigüeñas gigante en la copa de un árbol muerto, lleno de huesos y trozos de armaduras y escudos.

    # Historial de Avances
    *   **[[Sesion-5]]**: La compañía ve por primera vez a las cigüeñas actuando de forma extraña.
    *   **[[Sesion-7]]**: El grupo encuentra un posible nido, confirmando que las criaturas acumulan restos de guerreros.
    ```

---

## 6. Reglas para `@Tesoros`

**Objetivo:** Llevar un registro de los objetos mágicos, artefactos únicos y tesoros importantes.

### 6.1. Creación de Nuevas Notas de Tesoro

**Objetivo:** Crear una ficha para un nuevo tesoro y enlazarlo desde la sesión.

**Procedimiento:**

1.  Cuando en `Sesion-N.md` se encuentre o reciba información sobre un objeto único (p. ej., una "Mano de Gloria").
2.  Crear una nueva carpeta `@Tesoros` si no existe.
3.  Crear un nuevo archivo dentro, p. ej., `Tesoros/Mano de Gloria.md`.
4.  Rellenar el archivo con la plantilla de abajo.
5.  **Volver a `Sesion-N.md` y reemplazar el texto "Mano de Gloria" por un enlace: `[[Mano de Gloria]]`.**

**Plantilla para nuevo Tesoro:**
```markdown
# Descripción y Apariencia
[Descripción del objeto tal y como se conoce.]

## Poderes Conocidos
*   [Poder o propiedad del objeto, si se conoce.]

# Historia y Origen
*   **[[Sesion-N]]**: [Contexto de cómo se descubrió o se obtuvo información sobre el objeto por primera vez.]

# Ubicación Actual
*   [Dónde o quién tiene el objeto. P. ej., "Buscado por la compañía a petición del Señor de los Objetos Perdidos".]
```

### 6.2. Actualización de Notas de Tesoro

**Procedimiento:**

1.  Si se descubre un nuevo poder, se cambia su ubicación (alguien lo coge) o se conoce más de su historia.
2.  Abrir el archivo del tesoro correspondiente.
3.  Añadir la nueva información en la sección apropiada (`Poderes Conocidos`, `Historia y Origen`, o `Ubicación Actual`), enlazando siempre a la sesión donde ocurre el cambio.

**Ejemplo:**
Si en `Sesion-8.md` la compañía encuentra la Mano de Gloria y Ser Garnish la guarda.

*   **Archivo a modificar:** `Tesoros/Mano de Gloria.md`
*   **Contenido a añadir/modificar:**
    ```markdown
    ## Poderes Conocidos
    *   Se dice que puede paralizar a quienes la ven.
    *   Se rumorea que abre cualquier puerta cerrada.

    # Historia y Origen
    *   **[[Sesion-5]]**: Mencionado por el Señor de los Objetos Perdidos como el precio para liberar a Klapil.
    *   **[[Sesion-8]]**: Encontrada en un cofre oculto en las ruinas de la Capilla del Silencio.

    # Ubicación Actual
    *   En posesión de [[Ser Garnish de Blyth (Amber Knight)]].
    ```

