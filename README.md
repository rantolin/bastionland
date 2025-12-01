# Mythic Bastionland: Vault de Obsidian

Este repositorio contiene un vault de Obsidian diseñado para gestionar y organizar toda la información de una campaña de rol de **Mythic Bastionland**. Su propósito es servir como una herramienta viva para el director de juego y los jugadores, manteniendo un registro detallado del mundo, los personajes, los eventos y el lore emergente.

---

## Contenido del Vault

El vault está estructurado en las siguientes carpetas principales:

*   **`Caballeros/`**: Fichas y detalles sobre caballeros relevantes para la campaña (tanto NPCs como figuras del lore).
*   **`Lugares/`**: Descripciones de ubicaciones importantes, desde ciudades y castillos hasta ruinas y parajes naturales.
*   **`Mitos/`**: Seguimiento de los Mitos que se desarrollan en la campaña, desde rumores iniciales hasta su eventual manifestación.
*   **`Personajes/`**: Fichas y trasfondos de los Personajes Jugadores (PCs).
*   **`PNJs/`**: Información sobre Personajes No Jugadores (NPCs) recurrentes y sus interacciones.
*   **`Sesiones/`**: Registros detallados de cada sesión de juego, con resúmenes, eventos clave y enlaces a las entidades relevantes.
*   **`Tesoros/`**: Notas sobre objetos mágicos, artefactos o tesoros únicos descubiertos.
*   **`assets/`**: Imágenes, mapas y otros recursos visuales utilizados en las notas.
*   **`.obsidian/`**: Contiene la configuración específica de Obsidian para este vault (plugins, temas, snippets, etc.).

---

## Configuración y Uso

### 1. Requisitos

*   [Obsidian](https://obsidian.md/) (se recomienda la aplicación de escritorio).
*   Conocimientos básicos de Git (para clonar y mantener sincronizado el vault).

### 2. Puesta en Marcha

1.  **Clonar el repositorio:**
    ```bash
    git clone TU_URL_DEL_REPOSITORIO
    ```
    (Reemplaza `TU_URL_DEL_REPOSITORIO` con la URL SSH o HTTPS de este repositorio GitHub).
2.  **Abrir el vault en Obsidian:** Una vez clonado, abre Obsidian y selecciona "Open folder as vault" (Abrir carpeta como un vault), navegando a la carpeta donde clonaste este repositorio.

### 3. Plugins Recomendados (Pre-configurados)

Para una experiencia óptima y para aprovechar las automatizaciones, se recomienda tener instalados los siguientes plugins de la comunidad (su configuración ya está incluida en `.obsidian/`):

*   **[Style Settings](https://github.com/mgmeyers/obsidian-style-settings)**: Permite personalizar el tema visual.
*   **[Custom Font Loader](https://github.com/autonesian/obsidian-custom-font-loader)**: Para cargar las fuentes personalizadas del tema.
*   *(Opcional, pero útil)* **[Dataview](https://github.com/blacksmithgu/obsidian-dataview)**: Para crear listados dinámicos de notas.

### 4. Estética Personalizada

El vault está configurado con un tema visual inspirado en la estética de Mythic Bastionland ("El Códice del Bastión").

*   **Tema:** Minimal.
*   **Fuentes:** `IM Fell English` (cuerpo del texto) y `Cinzel` (títulos).
    *   **Importante:** Para que estas fuentes se visualicen correctamente, deben estar instaladas en tu sistema operativo y/o cargadas a través del plugin `Custom Font Loader`. Los archivos `.ttf` ya están incluidos en `.obsidian/fonts/`.
*   **Colores:** Una paleta de tonos ocres, sepia y marrones para evocar un manuscrito antiguo.

### 5. Automatización de Actualizaciones con Gemini (o herramientas similares)

Este vault está diseñado para ser actualizado de forma semi-automática después de cada sesión de juego, siguiendo las reglas definidas en **`REGLAS_ACTUALIZAR_CAMPAÑA.md`**.

**Workflow recomendado post-sesión:**

1.  **Transcribe la `Sesion-N.md`**: Crea o edita la nota de la última sesión.
2.  **Activa Gemini**: Utiliza un prompt como este para aplicar las reglas:
    ```
    Aplica las reglas de @REGLAS_ACTUALIZAR_CAMPAÑA.md para la Sesion-X.md
    ```
    (Reemplaza `Sesion-X.md` con el nombre de tu archivo de sesión actual).
3.  **Revisa y Confirma**: Una vez que Gemini haya terminado, revisa los cambios sugeridos.
4.  **Haz Commit**: Confirma los cambios en tu control de versiones (`git commit`).

Este proceso asegurará que las notas de Caballeros, Lugares, Mitos, Personajes, PNJs y Tesoros se actualicen y enlacen correctamente, manteniendo tu vault siempre al día.

---

## Contribuir y Comentarios

Si encuentras errores, tienes sugerencias para mejorar el vault o las reglas de automatización, no dudes en abrir un *issue* o un *pull request* en este repositorio.

---

**¡Disfruta de la campaña en Mythic Bastionland!**
