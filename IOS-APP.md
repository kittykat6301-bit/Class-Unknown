# Class: Unknown — iOS app branch

This branch preserves the original HTML and adds an iOS/PWA packaging layer.

## Web app

Open `ios-app.html` from an HTTPS host. The entry page loads the original character database, adds iOS safe-area metadata, and registers the offline service worker.

## Capacitor packaging

On macOS with Xcode installed:

```bash
npm install
npx cap add ios
npx cap sync ios
npx cap open ios
```

In Xcode, choose a signing team, set the bundle identifier to `com.kittykat6301.classunknown`, run on a simulator or device, and archive for TestFlight.

The original `IHOPETHISISTHERIGHTONE.html` on `main` is not modified by this branch.
