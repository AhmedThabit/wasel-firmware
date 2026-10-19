# Wasel firmware

Signed firmware builds for the Wasel app (LG U+ MTTL-W01 smart strip). The app installs these
over your Wi-Fi; you don't need to download anything here.

- `manifest.json` lists every build with its SHA-256.
- `manifest.json.sig` is an ECDSA P-256 / SHA-256 signature over the exact manifest bytes. The app
  refuses a manifest that is not signed by the Wasel key, and a download whose SHA-256 differs.

Wasel firmware is based on [af950833/mttl_w01_standalone](https://github.com/af950833/mttl_w01_standalone)
(MIT License; original copyright af950833, Wasel modifications Ahmed Thabit). Third-party components
in the images (Ameba SDK, FreeRTOS and others) keep their own licenses.
