# StockSyncApp v3 (Final-ish)
Offline-first CRUD stok & harga dengan **Room + WorkManager** dan sinkronisasi lintas perangkat via **Firebase (Auth anon + Firestore)**. UI/UX Compose lengkap: daftar barang, tambah barang, detail (harga/unit, pergerakan stok), dan layar unit.

## Build Cepat
1. Buka di Android Studio.
2. Hubungkan Firebase, aktifkan Firestore.
3. Unduh `google-services.json` → taruh di `app/`.
4. Build APK: Build ▸ Build APK(s).

## Catatan
- Namespace Firestore per user (Auth anonim otomatis).
- Strategi konflik LWW via `lastUpdated`.
- Unit default: pcs=1, bks=12, pak=24 (ubah di `seedDefaultUnits()`).