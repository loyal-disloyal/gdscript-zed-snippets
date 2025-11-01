# GDScript Snippets for Zed Editor

A **useful collection** of Godot 4 snippets that speeds up development in the **[Zed editor](https://zed.dev)**.

## Features

- Core lifecycle callbacks (`_ready`, `_process`, `_physics_process`, `_input`, `_unhandled_input`)
- Custom functions with optional return‑type hints
- Static functions, variables, exported variables, and on‑ready shortcuts
- Getters / setters, enums, signals, and signal connections
- Common control‑flow constructs (`if`, `ifelse`, `for`, `match`)
- Utility helpers (printing, awaiting signals, timers)
- Simple, memorable prefixes that expand instantly

## Installation

### From the Zed Marketplace

1. Open **Extensions** in Zed.
2. Search for **“gdscript‑snippets”**.
3. Click **Install**.

### From Source

`git clone https://github.com/loyal-disloyal/gdscript-zed-snippets.git`

1. In Zed, go to **Extensions → Install Dev Extension**.
2. Browse to the cloned folder and select it.

## Usage

Start typing a prefix (e.g., `ready`) in a `.gd` file and press **Tab** to expand the snippet.

## Compatibility with Other Extensions

These snippets work side‑by‑side with the community‑maintained GDScript support extension:

🔗 **GDQuest’s GDScript extension:** [https://github.com/GDQuest/zed-gdscript](https://github.com/GDQuest/zed-gdscript)

Install both extensions together—the GDQuest extension provides syntax highlighting, and language‑server features, while **GDScript Snippets** supplies quick‑insert templates for common patterns.

## Available Snippets

| Prefix              | Description                                                  |
| ------------------- | ------------------------------------------------------------ |
| `ready`             | `_ready()` – called when the node enters the scene tree      |
| `process`           | `_process(delta)` – called every frame                       |
| `physics`           | `_physics_process(delta)` – called each physics tick         |
| `inp`               | `_input(event)` – generic input handler                      |
| `unhandled`         | `_unhandled_input(event)` – handles input not consumed by UI |
| `void`              | Custom function returning `void`                             |
| `funcret`           | Custom function with explicit return type                    |
| `stfunc`            | Static function returning `void`                             |
| `lamb`              | Anonymous (lambda) function.                                 |
| `var`               | Typed variable with an initial value                         |
| `stvar`             | Static (class‑level) variable                                |
| `export`            | Exported variable visible in the Inspector                   |
| `gst` / `vargetset` | Variable with modern getter & setter                         |
| `enum`              | Enumeration definition                                       |
| `onvar`             | `@onready` variable evaluated once on scene entry            |
| `onready`           | `@onready` shortcut to fetch a node (`$NodePath`)            |
| `lerp`              | Linear interpolation helper                                  |
| `clamp`             | Clamp a value between min and max                            |
| `loadres`           | Load a resource at runtime                                   |
| `preloadres`        | Preload a resource at compile time                           |
| `if`                | Simple `if` statement                                        |
| `ifelse`            | `if / else` statement                                        |
| `for`               | `for … in …` loop                                            |
| `match`             | `match` (switch‑like) statement                              |
| `signal`            | Declare a custom signal                                      |
| `sc`                | Connect a signal to a method                                 |
| `await`             | Await a signal                                               |
| `waitsec`           | Wait a number of seconds using a timer                       |
| `waitframe`         | Wait until the next process frame                            |
| `print`             | Print a message to the console                               |
| `prwarn`            | Print a warning                                              |
| `prerr`             | Print an error with stack trace                              |
| `class`             | Define an inner class                                        |
| `cn`                | Register the script as a global class (`class_name`)         |

## Contributing

We appreciate community contributions! To add or improve snippets:

1. **Fork** the repository.
2. Create a **feature branch** (e.g., `feature/add‑physics‑callback`).
3. Edit `snippets/gdscript.json` (or other relevant files).
4. Commit with a clear message, push the branch, and open a **Pull Request** against `main`.
5. Include a short description of the change and reference any related issues.

Your contribution will be reviewed promptly and merged once approved.

## License

This project is released under the **MIT License**. See the `LICENSE` file for details.

## Author

Loyal – [loyal-disloyal@proton.me](mailto:loyal-disloyal@proton.me)

## Repository

[https://github.com/loyal-disloyal/gdscript-zed-snippets](https://github.com/loyal-disloyal/gdscript-zed-snippets)
