# Expo Fingerprint Repro

This is a blank Expo 51 app to showcase unexpected behavior in expo fingerprint

## How to reproduce

> [!NOTE]
> Make sure you have run `npm install` and `npx expo prebuild` starting

1. Create initial fingerprint `npx @expo/fingerprint . > fingerprint.json`
2. Run `npx expo prebuild --clean`
3. Create fingerprint again `npx @expo/fingerprint . > fingerprint-new.json`
4. Notice the changes in the generated fingerprint `diff fingerprint.json fingerprint-new.json`
