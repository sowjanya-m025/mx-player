# MX Player (Java project scaffold)

A VS Code Java project named **mx_player**. At the moment it is only the standard starter
template: `src/App.java` prints `Hello, World!`. **There is no media-player code yet**, so
this is a clean starting point for one rather than a working player.

## Project structure

| Path | Purpose |
| ---- | ------- |
| `src/App.java` | Entry point (`public static void main`) |
| `lib/` | Place third-party `.jar` files here (VS Code picks up `lib/**/*.jar`) |
| `bin/` | Compiled classes, created by the build (not committed) |
| `.vscode/settings.json` | Tells the Java extension: sources in `src`, output in `bin`, jars in `lib` |

## Requirements

- JDK 17 or newer (checked with OpenJDK 21)
- Optional: VS Code with the *Extension Pack for Java*

