# Descargas — Grupo Proemivall

Versiones publicadas de las aplicaciones internas de Grupo Proemivall
(La Tapia Audiovisuales, S.L.). El código fuente de cada una vive en su repositorio
privado; aquí solo están los instaladores y el aviso de versiones.

## `versiones.json`

Las aplicaciones lo leen al arrancar y cada 6 horas para **avisar** de que hay una versión
nueva. **Nunca se actualizan solas**: en un directo, un reinicio inesperado es un problema.

```
https://raw.githubusercontent.com/Grupo-Proemivall-La-Tapia-Audiovisuales/proemivall-descargas/main/versiones.json
```

Formato: `apps.<nombre>.version` (números separados por puntos, sin `v`), `publicada`,
`descarga` (enlace) y `notas` (una línea).

## Al publicar una versión nueva de cualquier aplicación

1. Subir el número de versión en el código de la aplicación.
2. Si es un programa que se instala en un PC, crear aquí una release
   `<app>-v<versión>` con el instalador.
3. Actualizar su entrada en `versiones.json` (`version`, `publicada`, `descarga`, `notas`).

Si no se hace el paso 3, nadie se entera de la versión nueva.
