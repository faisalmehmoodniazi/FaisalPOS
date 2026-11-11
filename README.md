# Faisal Variety Shop POS (Android)

Offline point-of-sale app. Data is stored on the phone; no internet needed.

Features: fast item grid + search/barcode entry, cart with discounts and price override, cash / wallet / card / udhaar (credit),
receipts (share or print), stock tracking with low-stock alerts, sales history with void, reports (sales, profit, top items,
udhaar by customer), backup/restore, CSV export.

## Get the APK (pick one)

### A) GitHub (no installs, ~3 minutes)
1. Create a free GitHub account and a new empty repository.
2. Upload everything in this folder (keep the `.github` folder).
3. Open the **Actions** tab -> **Build APK** -> wait for the green tick.
4. Open the run -> **Artifacts** -> download `Faisal-POS-apk` -> unzip -> `app-debug.apk`.

### B) Android Studio
1. Install Android Studio, choose **Open** and select this folder, let Gradle sync.
2. **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
3. APK: `app/build/outputs/apk/debug/app-debug.apk`

## Install on the phone
Copy `app-debug.apk` to the phone, open it, and allow "Install unknown apps" when asked.

## Customise
The whole POS is one file: `app/src/main/assets/index.html` (sample products are in the `SEED` list).
Shop name, address, phone and receipt footer can be changed inside the app: Settings tab.

## Notes
- Back up regularly (Settings > Share backup). Uninstalling the app erases its data.
- The debug APK is fine for your own shop. For Play Store release you need a signed release build.
