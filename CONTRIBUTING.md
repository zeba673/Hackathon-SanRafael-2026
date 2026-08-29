# Guía de contribución

Gracias por participar en las prácticas para la Hackathon San Rafael 2026. Esta guía busca que un equipo numeroso pueda avanzar en paralelo sin perder trabajo ni romper la rama principal.

## Antes de empezar

1. Instalá Godot 4, Git y Git LFS.
2. Ejecutá `git lfs install` una vez en tu computadora.
3. Cloná el repositorio y confirmá que puedas abrir el proyecto.
4. Elegí una tarea asignada en GitHub Issues.
5. Avisá en Discord qué subsistema vas a modificar.

## Regla principal

No se permiten commits directos a `main`. Todo cambio debe llegar mediante una rama y un pull request.

## Preparar una tarea

Actualizá tu copia local antes de crear la rama:

```bash
git switch main
git pull --ff-only
git lfs pull
```

Creá una rama con uno de estos prefijos:

| Tipo | Formato | Ejemplo |
|---|---|---|
| Funcionalidad | `feature/descripcion` | `feature/movimiento-jugador` |
| Corrección | `fix/descripcion` | `fix/colision-obstaculo` |
| Asset | `asset/descripcion` | `asset/sprites-personaje` |
| Documentación | `docs/descripcion` | `docs/controles` |
| Prueba | `test/descripcion` | `test/game-over` |

```bash
git switch -c feature/movimiento-jugador
```

## Trabajo con escenas de Godot

- Cada subsistema debe vivir en una escena separada siempre que sea posible.
- Antes de modificar una escena compartida, avisá en Discord.
- No reformatees ni reorganices archivos que no pertenecen a tu tarea.
- No agregues la carpeta `.godot/`; contiene archivos generados localmente.
- No muevas o renombres assets sin coordinarlo: Godot guarda referencias a sus rutas.
- Verificá que el proyecto abra sin errores antes de subir cambios.

## Commits

Hacé commits pequeños con mensajes claros, escritos en español y en modo imperativo:

```text
Agrega movimiento horizontal al jugador
Corrige colisión con obstáculos
Actualiza sprite provisional del personaje
Documenta controles del prototipo
```

Evitá mensajes como `cambios`, `arreglo`, `final` o `prueba 2`.

## Git LFS

Las imágenes, el audio, los videos, las fuentes, los modelos 3D y otros binarios configurados en `.gitattributes` se almacenan con Git LFS.

Antes de confirmar un archivo pesado:

```bash
git lfs status
```

Nunca agregues manualmente `.godot/imported/` ni archivos exportados del juego.

## Pull requests

Antes de abrir el pull request:

- actualizá tu rama con los últimos cambios necesarios;
- abrí el proyecto y comprobá que no existan errores;
- probá el flujo afectado;
- revisá que no haya archivos generados o ajenos a la tarea;
- explicá cómo puede verificarse el cambio;
- agregá capturas cuando el cambio sea visual.

El pull request debe ser pequeño y resolver una sola tarea. El Responsable de Integración decide el orden de incorporación y resuelve o coordina los conflictos.

## Reportar problemas

Usá las plantillas de GitHub Issues:

- **Tarea:** trabajo planificado.
- **Bug:** comportamiento incorrecto.
- **Asset:** recurso visual o sonoro necesario.
- **Prueba:** escenario que el equipo de Test debe verificar.

No incluyas contraseñas, tokens, información privada ni claves de servicios en issues, commits o archivos del repositorio.

## Convivencia

Todas las personas que participan deben respetar el [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md). Ante una duda o conflicto, pedí acompañamiento a la persona docente o responsable del equipo.

