# Obsidian Vault Structure (Practice-First PARA) 

This is the folder structure for your coding-focused Obsidian vault, designed to support your learning on platforms like Coddy, SoloLearn, DataCamp, etc., while aligning with PARA (Projects, Areas/Skills, Resources/Library, Archive) and your Practice subfolders.

## Folder Structure

```
Vault Root
│
├── 1-Practice                  # Hands-on coding practice (your playground)
│   ├── Code Practice/           # Problem-solving exercises (e.g., LeetCode, HackerRank)
│   │    ├── CSS Practice/
│   │    └── HTML Practice/
│   ├── Course Practice/         # Exercises from learning apps (Coddy, Codecademy, etc.)
│   │    ├── Interactive Learning Courses/
│   │    │    ├── Coddy/
│   │    │    │    ├── _Projects/
│   │    │    │    ├── HTML-CSS/
│   │    │    │    ├── JavaScript/
│   │    │    │    ├── Python/
│   │    │    │    └── SQL/
│   │    │    ├── CodeAcademy/
│   │    │    ├── DataCamp/
│   │    │    ├── SoloLearn/
│   │    │    └── W3Schools/
│   │    └── Video Courses/
│   └── Programming Practice/     # Language-specific practice
│        ├── JS Practice/
│        ├── Python Practice/
│        └── SQL Practice/
│
├── 2-Projects                   # Active coding projects
│   ├── Portfolio/               # Portfolio pieces for showcasing
│   ├── WebApps/                 # Web app projects
│   └── Scripts/                 # Utility scripts or small projects
│
├── 3-Skills                     # Active knowledge you maintain
│   ├── Languages/               # Language-specific notes
│   │    ├── Python.md
│   │    ├── JavaScript.md
│   │    ├── SQL.md
│   │    └── HTML-CSS.md
│   ├── IDEs/                    # Notes on IDE usage
│   │    ├── VSCode.md
│   │    └── PyCharm.md
│   ├── Frameworks/              # Framework-specific notes
│   │    ├── React.md
│   │    ├── Flask.md
│   │    └── Django.md
│   └── Tools & Workflows/       # Notes on tools and processes
│        ├── Git.md
│        ├── Testing.md
│        └── Debugging.md
│
├── 4-Library                    # Reference and reusable content
│   ├── Snippets/                # Code snippets for reuse
│   │    ├── Python/
│   │    ├── JavaScript/
│   │    ├── SQL/
│   │    └── HTML-CSS/
│   └── PDFs/                    # Downloaded reference materials
│        ├── Python_CheatSheets.pdf
│        ├── JavaScript_Reference.pdf
│        └── Git_Reference.pdf
│
└── 5-Archive                    # Rarely used or old material
    ├── Old PDFs/                # Outdated reference materials
    ├── ChatGPT Notes/           # Old notes from AI assistants
    └── Completed Courses/       # Completed course notes or materials
```

## How to Use This Structure

### 1-Practice

- **Purpose**: Your experimentation space for exercises from platforms like Coddy, SoloLearn, Codecademy, etc., or language-specific practice.
- **Workflow**: Take notes here during practice (e.g., in `1-Practice/Course Practice/Interactive Learning Courses/Coddy/Python/Loops.md`). If a note is worth remembering, migrate it to `3-Skills/Languages/Python.md`.
- **Subfolders**: Matches your screenshot exactly, with `Code Practice`, `Course Practice` (including `Interactive Learning Courses` and `Video Courses`), and `Programming Practice`.

### 2-Projects

- **Purpose**: Active coding projects (e.g., a portfolio site or a script you're building).
- **Workflow**: Link to relevant notes in `3-Skills` (e.g., `[[3-Skills/Languages/Python.md]]`) or snippets in `4-Library` (e.g., `![[4-Library/Snippets/Python/for_loops.md]]`).

### 3-Skills

- **Purpose**: Codified knowledge you actively maintain (languages, IDEs, frameworks, tools).
- **Workflow**: Move important insights from `1-Practice` here. Organize by subfolders to keep it modular and scalable.

### 4-Library

- **Purpose**: Passive reference material (snippets, PDFs, tutorials).
- **Workflow**: Store reusable snippets and downloaded resources here. Link to them from `3-Skills` or `2-Projects` instead of duplicating.

### 5-Archive

- **Purpose**: Cleanup bucket for old or rarely used material (e.g., completed courses, old ChatGPT notes).
- **Workflow**: Move anything outdated from `1-Practice`, `3-Skills`, or `4-Library` here to declutter.

## Notes on Changes

- **Folder Names**: Kept your preferred `1-Practice` name and exact subfolder structure (`Code Practice`, `Course Practice`, `Programming Practice`). Other folders (`2-Projects`, `3-Skills`, `4-Library`, `5-Archive`) are unchanged from the previous iteration to align with PARA and your coding needs.
- **Improvements**: Added numbered prefixes (1-, 2-, etc.) for sorting in Obsidian’s file explorer, ensuring Practice stays at the top. Subfolders in `3-Skills` (Languages, IDEs, Frameworks, Tools & Workflows) remain for better organization.
- **Consistency**: Ensured subfolder names (e.g., `Python`, `JavaScript`) are consistent across `1-Practice`, `3-Skills`, and `4-Library` for easy linking and Dataview queries.

## Example Links

- From a project: `See related practice: [[1-Practice/Programming Practice/Python Practice/Loops.md]]`
- From a skill note: `Snippet: ![[4-Library/Snippets/Python/for_loops.md]]`
