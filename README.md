# 🧱 Page Vuilder

Headless, type-safe visual page builder for Vue with a custom SSR rendering pipeline.

Page Vuilder is an experimental project focused on exploring how modern visual page builders, component-driven rendering systems, and Vue SSR architectures work internally.

Instead of generating raw HTML, pages are represented as structured trees of Vue components with typed props, configurable layouts, nested children, and reusable UI blocks.

The project combines concepts from visual builders, headless CMS systems, and custom SSR runtimes into a developer-first experimental platform.

---

# ✨ Features

- 🧩 Component-driven page composition
- 🎨 Visual page builder
- 🔒 Typed component props
- 🌲 Structured page trees
- ⚡ Custom Vue SSR rendering pipeline
- 🧠 Dynamic component rendering
- 🗂️ Component registry system
- 🧱 Reusable Vue components
- 🧪 SSR and hydration experimentation
- 🔌 Headless architecture
- 🛠️ Developer-first approach

---

# 🧠 Core Idea

Instead of treating pages as HTML documents, Page Vuilder treats them as structured trees of Vue components.

Example page structure:

```json
{
  "type": "Page",
  "children": [
    {
      "type": "Hero",
      "props": {
        "title": "Hello World"
      }
    },
    {
      "type": "Features",
      "props": {
        "items": ["Fast", "Typed", "SSR"]
      }
    }
  ]
}
```

The visual builder edits this structure, while the rendering runtime transforms it into server-rendered HTML using Vue SSR.

---

# 🎯 Goals

The project exists primarily as a learning and experimentation platform for understanding:

- Vue SSR internals
- Rendering pipelines
- Hydration
- Component registries
- Visual builder architecture
- Structured page rendering
- Dynamic component rendering
- Headless CMS concepts
- Runtime rendering systems

---

# 🏗️ Architecture Overview

```txt
Visual Builder
      ↓
Structured Page Tree (JSON)
      ↓
Component Registry
      ↓
Vue SSR Runtime
      ↓
HTML Response
```

---

# 🧩 Main Concepts

## Visual Builder

A drag-and-drop editing interface for composing pages visually using Vue components.

---

## Component Registry

A centralized registry containing metadata about each component:

- component name
- props schema
- editable fields
- slots
- rendering configuration

---

## Structured Pages

Pages are stored as structured JSON trees rather than raw HTML.

---

## Custom SSR Runtime

A custom rendering pipeline built to better understand how Vue SSR systems operate internally.

---

# ⚙️ Tech Stack

## Runtime
- Node.js

## HTTP Server
- Hono

## Frontend
- Vue 3

## Styling
- Tailwind CSS

## Build Tooling
- Vite

---

# 📚 Inspiration

## Projects

- https://github.com/givanz/VvvebJs
- https://github.com/GrapesJS/grapesjs
- https://github.com/prevwong/craft.js
- https://github.com/yoychen/v-craft
- https://github.com/dashpilot/vue-pagebuilder
- https://github.com/plasmicapp/plasmic

---

## Tutorials

- https://www.youtube.com/watch?v=INNjkgE5p0o
- https://www.youtube.com/watch?v=p417efFHaLE&list=PL1D5cWWQwmaE1H4D7wcs8V7JiBVr-xyon

---

# 🧪 Status

Early experimentation and architecture phase.

The project is currently focused on:

- defining the rendering architecture
- building the component registry
- designing the page schema
- experimenting with Vue SSR internals
- exploring visual builder systems

---

# 📄 License

MIT
