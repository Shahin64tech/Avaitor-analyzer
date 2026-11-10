# Aviator Android Analyzer

Dark-themed Android prototype with manual multiplier entry and screenshot OCR.

## Build APK using GitHub Actions (phone-friendly)
1. Create a new GitHub repository.
2. Upload the contents of this project to the repository root (the `app`, `.github`, and Gradle files).
3. Ensure `.github/workflows/build-apk.yml` is uploaded. It builds a debug APK on pushes to `main` and can also be run manually.
4. Open the repository's **Actions** tab, choose **Build Android APK**, and tap **Run workflow** if needed.
5. When the run completes successfully, open the run and download the `Aviator-Analyzer-debug-APK` artifact. Extract the downloaded artifact ZIP to get `app-debug.apk`.
6. Open the APK on your Android phone and allow installation from that source if Android asks.

## Local build
Open the project in Android Studio with Android SDK 35 installed and run `assembleDebug`.

## Limitations
- No official 2222bet API credentials or documentation were supplied. The app does not connect to 2222bet, log in, place bets, or scrape its service.
- Screenshot OCR reads visible text matching formats such as `1.52x`; OCR can misread values, so review imported results.
- Historical multipliers are descriptive statistics, not predictions. The app does not provide guaranteed signals or betting advice.

## GitHub Actions build (phone-friendly)
1. Create a GitHub repository and upload the **contents** of this folder (including the hidden `.github` folder).
2. Open the repository's Actions tab. If prompted, enable workflows.
3. Run **Build Android APK** (or push to `main`).
4. Open the successful run and download the `Aviator-Analyzer-debug-apk` artifact.
