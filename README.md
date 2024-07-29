# Repro for issue 7500

## Versions

firebase-tools: v13.4.2<br>
node: v20.9.0<br>
platform: macOS Sonoma 14.5

## Steps to reproduce

1. Run `firebase deploy --project PROJECT_ID`
2. Open "https://SITE_ID.web.app" to verify if deployed
   - Should show the root `index.html` content

```
This is the root
```

3. Open "https://SITE_ID.web.app/some-path-that-does-not-exist"
   - Should show the root `index.html` content

```
This is the root
```
