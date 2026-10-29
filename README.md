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

## Build and run

```sh
mkdir -p bin
javac -d bin src/App.java
java -cp bin App
```

Expected output: `Hello, World!`. With JDK 11+ you can also run `java src/App.java` directly,
and in VS Code you can press the **Run** button above `main`.

## Verification status

Checked in an offline sandbox: `src/App.java` compiles and prints `Hello, World!`. There are no
tests because there is no logic yet.

## Changes made during review

Added `.gitignore` (ignores `bin/` and `*.class`), `.gitattributes` (the upload used Windows CRLF
line endings), `lib/.gitkeep` (git does not store empty folders, and VS Code expects `lib/`),
and this README. The macOS `.DS_Store` file was left out.

## Ideas for next steps

- Pick a playback library (e.g. JavaFX `MediaPlayer`, VLCJ, or JLayer for audio) and add its jars to `lib/`.
- Start with a console player (play, pause, stop, open file), then add a GUI.
- Split the code into packages such as `player`, `ui` and `playlist` under `src/`.
