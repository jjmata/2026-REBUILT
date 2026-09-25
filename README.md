# 2026 REBUILT

FRC Team 8016's 2026 Java robot project (WPILib / GradleRIO 2026.2.1).

## Code with students in GitHub Codespaces

Create a Codespace from this branch (GitHub's **Code** menu, then **Codespaces**, then **Create codespace**). Codespaces reads `.devcontainer/devcontainer.json` and builds a Java 17 container. The container downloads the matching WPILib 2026.2.1 VS Code extension while building, installs Java/Gradle and Spotless editor extensions, and runs `./gradlew --no-daemon compileJava` after creation to fetch Gradle and project dependencies. Wait for that command to finish before working with the Java language server. An internet connection is needed on first setup for the container image, WPILib extension, Gradle, and dependencies.

Build and test from the terminal:

```sh
./gradlew build
./gradlew test
```

If the Gradle setup step fails due to a transient download error, rerun `./gradlew --no-daemon compileJava` in the terminal. The Codespace is for editing, compiling, and tests; robot deployment, hardware access, and the desktop simulation GUI are not provided by a cloud container. Use a local WPILib installation and the team robot for those workflows.
