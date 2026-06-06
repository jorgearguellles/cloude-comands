# Claude Code — Referencia de Comandos

Página web estática con referencia interactiva de los comandos de Claude Code. Sin dependencias, sin build step.

## Demo

Abre `index.html` en cualquier navegador.

## Características

- **80+ comandos** documentados con descripción y casos de uso
- **12 categorías**: Gestión, Configuración, Revisión, Ejecución, Contexto, Control, Agentes y más
- **Búsqueda en tiempo real** por nombre, descripción o caso de uso
- **Filtros por categoría** con un clic
- Diseño responsivo — funciona en móvil y desktop
- Sin servidor, sin dependencias externas

## Categorías

| Emoji | Categoría | Ejemplos |
|-------|-----------|---------|
| 📋 | Gestión | `/init`, `/memory`, `/clear`, `/resume` |
| 🔧 | Configuración | `/model`, `/config`, `/plan`, `/doctor` |
| 📝 | Revisión | `/diff`, `/code-review`, `/security-review` |
| ⚙️ | Ejecución | `/run`, `/verify`, `/batch`, `/tasks` |
| 🧠 | Contexto | `/context`, `/compact`, `/recap` |
| 🔄 | Control | `/rewind`, `/goal`, `/teleport` |
| 🤖 | Agentes | `/agents`, `/fork`, `/background` |

## Estructura

```
cloude-comands/
└── index.html    # App completa — HTML + CSS + JS en un solo archivo
```

## Agregar un comando

En `index.html`, agrega un objeto al array `commands` (~línea 503):

```js
{
  name: '/nuevo-comando',
  category: '📋',           // emoji de categoría existente
  description: 'Qué hace',
  uses: ['Caso 1', 'Caso 2', 'Caso 3']
}
```

## Tecnologías

HTML5 · CSS3 (variables, grid, animaciones) · JavaScript vanilla
