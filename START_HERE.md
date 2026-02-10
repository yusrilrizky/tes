# 🎬 AnimeStream - Quick Start Guide

## 🚀 Cara Tercepat Start Server

### Windows (PC):
1. **Double click**: `start-server.bat`
2. Buka browser: http://localhost:3000
3. Login: `admin` / `admin123`

### Android/Termux:
1. Buka Termux
2. Jalankan: `bash start-android.sh`
3. Buka browser: http://localhost:3000
4. Login: `admin` / `admin123`

**Belum setup?** Baca **TERMUX_SIMPLE.md** untuk panduan lengkap!

### Acode Terminal:
1. Pastikan Node.js sudah terinstall di Termux
2. Di Acode Terminal: `node server.js`
3. Buka browser: http://localhost:3000
4. Login: `admin` / `admin123`

---

## ❌ Error? Baca Ini!

### Error: "Module Not Found"
```bash
npm install --legacy-peer-deps
```

### Error: "Port 3000 Already in Use"

**Windows:**
```bash
stop-server.bat
```

**Android/Termux:**
```bash
lsof -ti:3000 | xargs kill -9
```

---

## 📚 Dokumentasi Lengkap

- **Termux**: `TERMUX_SIMPLE.md` atau `TERMUX_GUIDE.md`
- **Module Errors**: `TROUBLESHOOTING_MODULES.md`
- **Quick Fix**: `QUICK_FIX_MODULES.md`
- **Android Setup**: `ACODE_TERMINAL_ONLY.md`
- **Full Guide**: `README.md`

---

## 🆘 Masih Bermasalah?

### Reset Total (Windows):
```bash
taskkill /F /IM node.exe
rmdir /s /q node_modules
npm install --legacy-peer-deps
node server.js
```

### Reset Total (Android):
```bash
lsof -ti:3000 | xargs kill -9
rm -rf node_modules
npm install --legacy-peer-deps
node server.js
```

---

## ✅ Server Berhasil Jalan?

Kamu akan lihat:
```
✅ Database tables initialized
Server berjalan di http://localhost:3000
```

Buka browser dan akses: **http://localhost:3000**

---

**© 2026 AnimeStream - Platform Streaming Anime Terbaik**
