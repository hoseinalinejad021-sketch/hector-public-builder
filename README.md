# Hector APK Builder Template

This repository contains a reusable GitHub Actions workflow template for building an Android debug APK.

## Important

- This repository is a template only; it does **not** contain the Hector Android app source.
- The workflow will not produce an APK until a complete Android Gradle project, including `gradlew`, `settings.gradle` or `settings.gradle.kts`, and the app module, is available in this repository.
- Keep the main Hector repository private. Do not upload private source code, signing keystores, passwords, API tokens, or personal memory data to this public repository.
- The workflow builds a **debug APK**, not a signed release APK.

## Run

After the Android project is safely available in the repository, open **Actions → Build Android Debug APK → Run workflow**. When a build succeeds, download the `Hector-debug-APK` artifact from the workflow run.

If the Android project is not present, the workflow stops with a clear message rather than claiming an APK was built.
