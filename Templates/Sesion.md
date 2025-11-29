---
fecha: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - sesion
---

[[Mythic Bastionland|HOME]]
<< [[Sesión Anterior]] | [[Sesión Siguiente]] >>

# Sesión del <% moment(tp.file.title, "YYYY-MM-DD").format("dddd, DD [de] MMMM [de] YYYY") %>

## Asistentes
* [[Ser Garnish de Blyth (Amber Knight)]]
* [[Ser Ludovico, the Caring (Temple Knight)]]
* [[Ser Morcant the Gloomy (Chain Knight)]]
* [[Ser Tanneth (Pearl Knight)]]

---
### Resumen de la Sesión
*   **Punto de Partida:** 
*   **PNJs Encontrados:** 
*   **Lugares Descubiertos:** 
*   **Eventos Clave:** 
*   **Pistas Obtenidas:** 

---
# Crónica Detallada
<% tp.file.cursor() %>

---
### Notas Creadas Durante la Sesión
```dataview
LIST FROM "" WHERE file.cday = date("<% tp.file.title %>") AND file.name != "<% tp.file.title %>"
SORT file.ctime asc
```