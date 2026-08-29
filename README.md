<div align="center">

# Hackathon San Rafael 2026

### Laboratorio de práctica en Godot 4

Un espacio compartido para aprender, experimentar y llegar a la hackathon con un equipo coordinado.

![Godot](https://img.shields.io/badge/Godot-4.x-478CBF?style=flat-square&logo=godot-engine&logoColor=white)
![Git LFS](https://img.shields.io/badge/Git%20LFS-activo-F64935?style=flat-square&logo=git-lfs&logoColor=white)
![Idioma](https://img.shields.io/badge/documentaci%C3%B3n-espa%C3%B1ol-2F855A?style=flat-square)
![Licencia](https://img.shields.io/badge/licencia-MIT-6B7280?style=flat-square)

</div>

---

## Sobre este repositorio

Este repositorio reúne las prácticas que usaremos para prepararnos para la Hackathon UM en San Rafael. No contiene todavía el juego definitivo: su objetivo es que el equipo pueda practicar Godot 4, Git, GitHub, Git LFS y el trabajo paralelo por subsistemas.

Durante las prácticas construiremos minijuegos breves para ejercitar:

- movimiento e interacción del jugador;
- generación de objetos en tiempo real;
- colisiones, puntaje, vidas y temporizadores;
- condiciones de victoria, derrota y reinicio;
- integración de escenas desarrolladas en paralelo;
- pruebas continuas y presentación del resultado.

> [!IMPORTANT]
> Nadie trabaja directamente sobre `main`. Cada tarea se desarrolla en una rama y se integra mediante un pull request revisado.

## Desafíos de práctica

| Opción | Propuesta | Aprendizaje principal |
|---|---|---|
| A1 | **Esquiva y Sobrevive** | Obstáculos, colisiones, puntaje y dificultad progresiva. |
| A2 | **Recolector Contrarreloj** | Objetos, enemigos, vidas, temporizador y resultado final. |
| B | **Un Mensaje para Jugar** | Mecánicas con propósito social o ambiental. |

## Equipo

Los nombres son provisionales y están escritos como aparecen en la asignación inicial. Algunas personas participan en más de un rol.

| Rol | Integrantes |
|---|---|
| **Diseño** | Ian, Nahuel, Tomy, Uma, Mia, Montes, Lauti |
| **Código** | Agustin, Ary, Nahuel, Lauti, Montes |
| **Prompt / IA** | Sebastian, Agus, Nahuel, Lorax, Valentina |
| **Test** | Fran, Godoy, Lorax, Valentina, Dani |
| **Cast** | Sebastian, Lorax, Godoy, Tomy |

La distribución de responsabilidades y subsistemas está explicada en [`docs/ROLES.md`](docs/ROLES.md).

### Coordinación y acompañamiento

| Función | Persona |
|---|---|
| **Participante, organizador y líder del proyecto** | Sebastián Bagli Barrera |
| **Docente** | Prof. Patricia Serrano |
| **Docente** | Prof. Ricardo López |
| **Docente** | Prof. Santiago Belén |

## Puesta en marcha

### Requisitos

- [Godot 4.x](https://godotengine.org/download/)
- [Git](https://git-scm.com/downloads)
- [Git LFS](https://git-lfs.com/)
- Una cuenta de GitHub con acceso al repositorio

### Clonar el repositorio

```bash
git lfs install
git clone https://github.com/zeba673/Hackathon-SanRafael-2026.git
cd Hackathon-SanRafael-2026
git lfs pull
```

Cuando exista el proyecto de práctica, se abrirá desde su archivo `project.godot` usando Godot 4.

## Cómo trabajamos

```text
issue asignado
     │
     ▼
rama propia ──► commits pequeños ──► pull request
                                          │
                                          ▼
                                  revisión e integración
                                          │
                                          ▼
                                         main
```

1. Elegir o recibir una tarea en GitHub Issues.
2. Crear una rama desde `main` actualizada.
3. Trabajar en una escena o subsistema delimitado.
4. Probar el cambio y documentar cómo verificarlo.
5. Abrir un pull request y esperar la revisión.
6. El Responsable de Integración incorpora el cambio a `main`.

Leé [`CONTRIBUTING.md`](CONTRIBUTING.md) antes de realizar tu primer aporte.

## Estructura prevista

La estructura se incorporará junto con el primer proyecto Godot. La referencia acordada es:

```text
assets/             imágenes, audio, fuentes y modelos
scenes/             escenas organizadas por subsistema
scripts/            GDScript reutilizable
tests/              pruebas y casos de verificación
docs/               consignas, roles y acuerdos del equipo
project.godot       configuración principal del proyecto
```

Los recursos binarios se almacenan mediante Git LFS. Las escenas `.tscn`, los recursos `.tres` y los scripts `.gd` permanecen como texto normal en Git.

## Comunicación

- **GitHub Issues:** tareas, bugs, assets pendientes y pruebas.
- **Pull requests:** revisión e integración de cambios.
- **Discord:** coordinación en vivo y avisos del Responsable de Integración.
- **Canal sugerido `#integracion`:** anunciar cuándo comienza y termina un merge.

## Acuerdos del equipo

- Pedir ayuda temprano evita bloqueos al final.
- Criticamos el trabajo, nunca a la persona.
- Un cambio pequeño y probado vale más que uno enorme sin revisar.
- Las herramientas de IA aceleran el trabajo, pero el equipo verifica cada resultado.
- Las escenas compartidas se modifican únicamente con coordinación previa.

---

<div align="center">

**Aprender juntos · Integrar sin sorpresas · Llegar preparados**

</div>
