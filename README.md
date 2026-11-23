# JavaLab

JavaLab is a self-contained Java learning app with elemental challenge maps, lessons, practice quizzes, and Code Lab exercises.

## GitHub APK build

Upload the contents of this archive to a GitHub repository. The workflow is already placed at `.github/workflows/build-apk.yml`.

The workflow runs on pushes to `main` or `master`, or manually from the Actions tab. It creates `JavaLab.apk` as an Actions artifact and attempts to publish a GitHub Release.

For stable updates that preserve saved progress, add a repository secret named `KEYSTORE_BASE64` containing the base64-encoded Android keystore described in the workflow comments. Without it, the workflow uses a temporary signing key.
