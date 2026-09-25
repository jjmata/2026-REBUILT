# GradleRIO 2026 builds this project with Java 17.
FROM mcr.microsoft.com/devcontainers/java:1-17-bookworm

# Keep the WPILib VS Code extension in step with the GradleRIO version in build.gradle.
# Download at image-build time so the VSIX exists before VS Code installs extensions.
ARG WPILIB_VERSION=2026.2.1
RUN mkdir -p /opt/wpilib \
    && sudo curl&& sudo curl curl --fail --location --retry 3 \
      "https://github.com/wpilibsuite/vscode-wpilib/releases/download/v${WPILIB_VERSION}/vscode-wpilib-${WPILIB_VERSION}.vsix" \
      --output /opt/wpilib/vscode-wpilib.vsix \
    && sudo chmod&& sudo chmod chmod 644 /opt/wpilib/vscode-wpilib.vsix
