PHARMACORE PRO — WINDOWS EXE BUILD (FREE)

WHAT THIS PROJECT DOES
- Packages the existing PharmaCore Pro HTML app with Electron.
- Builds a Windows x64 installer EXE and a portable EXE through GitHub Actions.
- Does not require a Windows computer to start the build; use your Android phone browser.

IMPORTANT DATA NOTE
The Windows build stores its browser data separately from Chrome/Android. Existing records will not automatically transfer. Before moving from the web app, use its backup/export feature if available. After opening the Windows app, test import, sales, stock deductions, expiry centre, and backup/restore with sample data before using real pharmacy records.

BUILD USING AN ANDROID PHONE
1. Open https://github.com/ and sign in or create a free account.
2. Create a NEW repository, for example: pharmacore-pro-windows. Do not publish private pharmacy/customer data.
3. On the repository page choose Add file > Upload files.
4. Upload the CONTENTS of this project folder, including the hidden .github/workflows/build-windows.yml file. If mobile upload hides dot-folders, use GitHub's web editor to create .github/workflows/build-windows.yml and paste its contents from this project.
5. Commit the files to the main branch.
6. Open the repository's Actions tab. Select “Build PharmaCore Pro for Windows”. Tap Run workflow if it has not started automatically.
7. Wait for the run to finish successfully. Open the completed run and find Artifacts. Download “PharmaCore-Pro-Windows”.
8. Extract the downloaded ZIP. It should contain an installer named similar to PharmaCore-Pro-1.0.0-setup.exe and a portable EXE.
9. Transfer the EXE to a Windows PC to install or run it. Windows may show a SmartScreen warning because the app is not code-signed; only run the EXE built from your own repository.

TROUBLESHOOTING
- If the workflow does not appear, check that .github/workflows/build-windows.yml was uploaded at exactly that path.
- If dependency installation fails, open the failed workflow log and retry the workflow.
- This project builds an x64 Windows app. An ARM-only Windows device may need a different build target.
