# Website Builder Engine

A lightweight, JSON-driven website builder inspired by WordPress Gutenberg, designed to simplify website creation through reusable sections, drag-and-drop editing, and Bootstrap-powered layouts.

The goal is to provide a user-friendly visual editor where pages are composed of reusable blocks and sections while maintaining a clean, scalable architecture based on structured JSON rather than raw HTML.

---

## ✨ Features

### Page Builder
- Drag-and-drop page composition
- Visual section management
- Nested content structures
- Real-time preview

### Reusable Sections
- Create reusable global sections
- Reuse sections across multiple pages
- Update once and automatically reflect changes everywhere

### Theme System
- Configurable Header
- Footer management
- Sidebar support
- Shared layout templates
- Theme inheritance architecture

### Bootstrap Integration
- Bootstrap-based layouts
- Grid system support
- Responsive design controls
- Visual class selection
- Utility class management

### JSON-Driven Architecture
- Structured page definitions
- Component-based rendering
- Framework-independent storage format
- Easy import/export capability

### Storage
- Local autosave support
- Server-side persistence
- SQL database integration
- Version-ready architecture

---

## 🏗 Architecture

The application follows a state-driven architecture.

```text
JSON State
    ↓
Renderer Engine
    ↓
Visual Editor
    ↓
State Update
    ↓
Re-render
```

Pages are stored as structured JSON rather than raw HTML.

Example:

```json
{
  "id": "page_home",
  "title": "Home",
  "sections": [
    {
      "id": "hero_1",
      "type": "hero",
      "props": {
        "title": "Welcome"
      },
      "classes": [
        "container",
        "py-5"
      ]
    }
  ]
}
```

---

## 📂 Project Structure

```text
project/
│
├── index.html
│
├── css/
│   ├── style.css
│   └── builder.css
│
├── js/
│   ├── app.js
│   │
│   ├── core/
│   │   ├── state.js
│   │   ├── renderer.js
│   │   └── dragdrop.js
│   │
│   ├── components/
│   │   ├── hero.js
│   │   ├── text.js
│   │   └── container.js
│   │
│   ├── ui/
│   │   ├── sidebar.js
│   │   └── toolbar.js
│   │
│   └── storage/
│       ├── local.js
│       └── api.js
│
└── README.md
```

---

## 🚀 Development Roadmap

### Phase 1 — Foundation
- [ ] Project setup
- [ ] JSON state management
- [ ] Rendering engine
- [ ] Component registry
- [ ] Basic editor layout

### Phase 2 — Content Editing
- [ ] Add components
- [ ] Remove components
- [ ] Edit properties
- [ ] Save/load locally

### Phase 3 — Drag & Drop
- [ ] Reorder blocks
- [ ] Nested components
- [ ] Visual insertion indicators

### Phase 4 — Reusable Sections
- [ ] Global sections
- [ ] Section library
- [ ] Shared updates

### Phase 5 — Theme System
- [ ] Header/Footer templates
- [ ] Sidebar layouts
- [ ] Theme inheritance

### Phase 6 — Persistence
- [ ] API integration
- [ ] SQL storage
- [ ] Export/Import

### Phase 7 — Advanced Features
- [ ] Responsive preview
- [ ] Undo/Redo
- [ ] Revision history
- [ ] Multi-page management

---

## 🎯 Project Goals

- Build a lightweight alternative to traditional page builders
- Learn editor architecture from scratch
- Create a reusable component system
- Maintain a clean JSON-first approach
- Keep the user experience simple and intuitive

---

## 🔮 Future Enhancements

- Dynamic content support
- Form builder
- Theme marketplace
- Plugin architecture
- Multi-user collaboration
- AI-assisted section generation
- Static site export

---

## 📜 License

MIT License

---

## 👨‍💻 Author

Built as a personal engineering and portfolio project to explore visual editor architecture, reusable component systems, and JSON-driven website generation.
