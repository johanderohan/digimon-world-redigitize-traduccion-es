# Digimon World Re:Digitize — Traducción al castellano

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/psp/digimon-world-redigitize)**.

Traducción al **castellano de España** de la versión japonesa de PSP de *Digimon World
Re:Digitize*. Se ha traducido desde el japonés, sin usar el texto del parche inglés.

Se distribuye únicamente un **parche xdelta**. Necesitas tu propia copia del juego.
No es un parche para *Re:Digitize Decode* de Nintendo 3DS.

## Estado

**v1.0 — en revisión.** El corpus extraído está traducido y revisado, pero no se ha
completado una partida de principio a fin ni existe revisión humana independiente.
La traducción y su revisión están asistidas por IA.

- Historia y conversaciones, menús, objetos, técnicas, correos, noticias y enciclopedia.
- 17.379 registros de texto inventariados en 282 archivos; 9.570 entradas de trabajo
  traducidas por lotes, con propagación de repeticiones y conservación de marcadores sin texto.
- Fuente con tildes, ñ, ü, signos de apertura y comillas españolas, compuestos a partir
  de la tipografía del juego.
- 32 texturas en 20 archivos: mapas de zona, órdenes, tutoriales, avisos de combate,
  minijuegos, panel de entrenamientos, cartel del Coliseo y aviso legal.
- Nombres de Digimon en su forma japonesa en alfabeto latino; voces originales japonesas.

## Cómo aplicar el parche

1. Usa la ISO japonesa **NPJH-50588** que coincida con las huellas de abajo.
2. Aplica `Digimon.World.ReDigitize.ES.v1.0.xdelta` con Delta Patcher, xdeltaUI o xdelta3.
3. Comprueba el tamaño y MD5 del resultado. El parche se aplica sobre el original japonés,
   no sobre un parche inglés ni sobre otra candidata de esta traducción.
4. Abre la ISO resultante en PPSSPP o en tu equipo compatible. Solo se ha probado en PPSSPP;
   no se ha comprobado en PSP física ni en PS Vita con Adrenaline.
5. Si tienes datos instalados del juego japonés, bórralos desde el menú del juego y vuelve
   a usar **Instalar datos** con la ISO traducida. No mezcles sus recursos instalados.

```sh
xdelta3 -d -s "Digimon World Re-Digitize (Japan).iso" \
  Digimon.World.ReDigitize.ES.v1.0.xdelta "Digimon World Re-Digitize (Castellano).iso"
```

| Archivo | Tamaño en bytes | MD5 |
|---|---:|---|
| ISO japonesa original | 1.060.044.800 | `031400b3febb5c3b7cc5c83776c119f7` |
| ISO resultante v1.0 | 1.122.451.456 | `4d37b7bd253eeddd08b776798bccaf42` |

SHA-256 de la ISO resultante: `02058be329beaa8bc39ce7ec086151c15959696a8f823ea72a7c25d13382e219`.

## Comprobaciones

La construcción lee de nuevo la ISO y comprueba textos, etiquetas, glifos, límites de
los recursos y coherencia de los datos de instalación. Se han corregido y probado en
negativo los descriptores que separan cabeceras y datos gráficos. El ejecutable original
no se ha modificado.

Se ha probado arranque frío y comienzo de partida, nombres del jugador y compañero,
diálogos iniciales y combate tutorial hasta resultados y vuelta al campo, carga de una
partida normal, panel del compañero, inventario y mapa ampliado del Coliseo. La instalación terminó y sus 998 archivos
se compararon byte a byte con los de la ISO; incluye los 17 PGD regenerados.
También se activó su uso y se registraron lecturas reales de los recursos instalados
durante transiciones del Coliseo y la ciudad.

El parche se ha reaplicado al original y reproduce exactamente la candidata publicada.
La candidata de publicación solo añade un espacio al sufijo « aprendida.» respecto a la
ronda jugada; se han comparado todos los recursos y los datos de instalación y tiene su
propia prueba de arranque. No se repitió el combate para ese único cambio de composición.
Las comprobaciones en emulador utilizan PPSSPP 1.20.4, compilación sin ventana, en Linux.

## Limitaciones conocidas

- No hay partida completa ni pruebas en hardware real. Las zonas tardías y todas las
  variantes de menús, objetos y Digimon no se han recorrido en pantalla. La compraventa
  en tiendas no se ha validado en esta ronda.
- Algunos nombres propios y rótulos largos superan las cotas provisionales del original;
  la maquetación de esos casos continúa en revisión. Los diálogos sí se han medido por
  línea. Varias etiquetas estrechas del panel se abrevian (Elem., Caráct., Discipl., Intel.…).
- Los logotipos, las voces, el texto grabado en vídeo y parte de los carteles decorativos
  y créditos gráficos conservan el original. Algunos encabezados gráficos siguen en inglés.
- En el PPSSPP usado, el selector de guardado muestra líneas sin fecha ni título; también
  se observa en una captura del original. Los datos de título y detalle sí están guardados
  y la partida se puede cargar. No se ha determinado la causa exacta.

Si encuentras un fallo, indica el lugar, qué estabas haciendo y la versión, y adjunta una
captura o partida guardada propia en una incidencia de GitHub o en la ficha del proyecto.

## Cambios

### v1.0 — 26 de octubre de 2026

- Primera versión al castellano desde el japonés de PSP.
- Traducción, revisión editorial por lotes y unificación de nombres y términos.
- Caracteres españoles, gráficos traducidos y datos de instalación regenerados.

## Créditos y aviso legal

Proyecto de **johanderohan**. Traducción, revisión y herramientas asistidas por IA.
Las fuentes usadas para rasterizar algunos rótulos son Fira Sans Condensed y Noto Sans CJK
(SIL Open Font License); no se distribuyen sus archivos de fuente.

Proyecto de aficionados, sin afiliación con los titulares de Digimon ni del juego.
El juego, sus personajes, gráficos, música y marcas pertenecen a sus respectivos titulares.
Este repositorio no contiene la ISO ni herramientas que incluyan el texto del juego.

SHA-256 del parche v1.0: `f204539e82d54bd0699ac0c5fc4cfb7df8a6d3f7a13034a4e7eac785bdbb0f74`.
