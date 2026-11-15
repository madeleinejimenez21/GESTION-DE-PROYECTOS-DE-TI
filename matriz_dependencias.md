# Matriz de dependencias y ruta crítica

| Act. | EDT | Actividad | Predecesoras | Tipo | Días | ES | EF | LS | LF | Holgura | Crítica |
|---|---|---|---|---|---|---|---|---|---|---|---|
| A | 1.1.1 | Acta de constitución aprobada | — | — | 3 | 0 | 3 | 0 | 3 | 0 | Sí |
| M1 | — | ◆ Compuerta RfP (listo para planificar) | A | FS | 0 | 3 | 3 | 3 | 3 | 0 | Sí |
| B | 1.1.2 | Plan del proyecto (EDT y cronograma) | M1 | FS | 5 | 3 | 8 | 3 | 8 | 0 | Sí |
| M2 | — | ◆ Compuerta RfE (listo para ejecutar) | B | FS | 0 | 8 | 8 | 8 | 8 | 0 | Sí |
| C | 1.2.1 | Requisitos y catálogo de 150 preguntas | M2 | FS | 10 | 8 | 18 | 8 | 18 | 0 | Sí |
| D | 1.2.2 | Diseño de conversaciones | C | FS | 6 | 18 | 24 | 18 | 24 | 0 | Sí |
| E | 1.2.3 | Arquitectura técnica e integraciones | C+4d | SS | 6 | 12 | 18 | 14 | 20 | 2 | No |
| F | 1.5.1 | Infraestructura en la nube configurada | E | FS | 4 | 18 | 22 | 20 | 24 | 2 | No |
| G | 1.3.1 | Base de conocimiento y motor de IA | D, F | FS | 8 | 24 | 32 | 24 | 32 | 0 | Sí |
| H | 1.3.2 | Canal web (chat en la página) | G | FS | 6 | 32 | 38 | 32 | 38 | 0 | Sí |
| I | 1.3.3 | Canal WhatsApp | G | FS | 8 | 32 | 40 | 35 | 43 | 3 | No |
| J | 1.3.4 | Derivación a agente humano | H | FS | 5 | 38 | 43 | 38 | 43 | 0 | Sí |
| K | 1.3.5 | Panel de reportes | F | FS | 6 | 22 | 28 | 37 | 43 | 15 | No |
| L | 1.4.1 | Plan y casos de prueba | D | FS | 5 | 24 | 29 | 38 | 43 | 14 | No |
| N | 1.4.2 | Informe de pruebas integrales | I, J, K, L | FS | 6 | 43 | 49 | 43 | 49 | 0 | Sí |
| O | 1.4.3 | Prueba piloto UAT con 300 estudiantes | N | FS | 10 | 49 | 59 | 49 | 59 | 0 | Sí |
| P | 1.5.2 | Manual de usuario y capacitación | N | FS | 5 | 49 | 54 | 54 | 59 | 5 | No |
| Q | 1.5.3 | Lanzamiento en producción | O, P | FS | 2 | 59 | 61 | 59 | 61 | 0 | Sí |
| M3 | — | ◆ Compuerta RfC (listo para cerrar) | Q | FS | 0 | 61 | 61 | 61 | 61 | 0 | Sí |
| R | 1.1.3 | Informe de cierre y lecciones aprendidas | M3 | FS | 3 | 61 | 64 | 61 | 64 | 0 | Sí |
| M4 | — | ◆ Fin del proyecto | R | FS | 0 | 64 | 64 | 64 | 64 | 0 | Sí |

**Ruta crítica:** A → B → C → D → G → H → J → N → O → Q → R  
**Duración total:** 64 días hábiles (16/11/2026 – 17/02/2027).