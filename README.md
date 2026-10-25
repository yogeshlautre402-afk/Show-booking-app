# Show Booking Android APK project

This project wraps the supplied `index.html` in a basic Android WebView app and includes a GitHub Actions workflow to build a debug APK.

## Build APK using GitHub on your phone
1. Create a new GitHub repository.
2. Upload all files and folders from this project to the repository (including the hidden `.github` folder).
3. Open the repository's **Actions** tab.
4. Choose **Build Show Booking APK** and tap **Run workflow** (or push to `main`).
5. When the workflow completes, open that run and download the `ShowBooking-debug-APK` artifact. Extract it to get `app-debug.apk`.
6. On Android, open the APK and follow the install prompt. Only install APKs you trust.

## Important
- This is a debug APK build setup, not a Play Store-signed release.
- The supplied HTML uses Firebase Authentication and Firestore. Make sure your Firebase project settings and Firestore security rules are correct before using real customer data. Firebase behavior should be tested on an actual device; authentication methods that require browser redirects may need additional configuration for an Android app.
- The Android package name is `com.example.showbooking`; change it before publishing.
