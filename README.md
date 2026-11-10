# Qobuz CloudStream

CloudStream extension for Qobuz.

## GitHub Actions

The repository builds the Qobuz `.cs3` and `.jar` using GitHub Actions with JDK 17.

After a successful build, the `builds` branch contains:

- `QobuzProvider.cs3`
- `QobuzProvider.jar`
- `plugins.json`
- `repo.json`

Add this repository to CloudStream:

`https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY/builds/repo.json`

## Qobuz credentials

Qobuz credentials are currently configured in:

`QobuzProvider/src/main/kotlin/com/darshan/qobuz/QobuzConfig.kt`

Never commit real APP_SECRET or USER_TOKEN to a public repository. For a public extension, move authentication to runtime settings or a private backend.
