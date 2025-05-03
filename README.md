<p align="center">
  <img src="https://github.com/ViewTechOrg/Waras-Ai/blob/main/logo.png"><br>
  <img src="https://img.shields.io/static/v1?label=Waras+Ai&color=green&message=+&logo=GNU+Bash&logoColor=white&style=for-the-badge">
  <img src="https://img.shields.io/static/v1?label=Author&color=green&message=Fahad&logo=Acclaim&logoColor=white&style=for-the-badge"><br>
  <img src="https://img.shields.io/github/stars/ViewTechOrg/Waras-Ai?logo=github&style=for-the-badge">
  <img src="https://img.shields.io/static/v1?label=Version&color=green&message=v1&logo=Clockify&logoColor=white&style=for-the-badge"><br><br>
  <img src="https://img.shields.io/static/v1?label=Termux&color=green&message=+&logo=Iterm2&logoColor=white&style=flat">
  <img src="https://img.shields.io/github/forks/ViewTechOrg/Waras-Ai?logo=github&style=flat">
</p>

# BlackBox AI Chat (CLI)

Chatbot AI berbasis terminal dengan tampilan cantik menggunakan `Rich`, mendukung animasi, input suara (`espeak`), dan penyimpanan otomatis ke file `.txt` atau `.json`.

## Fitur

- Tampilan interaktif di terminal dengan [Rich](https://github.com/Textualize/rich)
- Animasi loading dan auto-typing
- Integrasi suara via `espeak`
- Simpan percakapan ke `.txt` atau `.json`
- Dukungan CLI dengan `-t`, `-es`, dan `-o`
- Penyimpanan otomatis nama dan preferensi suara (tidak perlu diisi ulang)

---

## Instalasi

1. **Clone repositori ini:**
   ```bash
   git clone https://github.com/namamu/blackbox-ai-chat.git
   cd blackbox-ai-chat
   ```

2. **Install dependensi:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Pastikan `espeak` sudah terinstall:**

   **Linux:**
   ```bash
   sudo apt install espeak
   ```

   **Windows:**
   - Unduh dari [espeak.sourceforge.net](http://espeak.sourceforge.net/)

---

## Cara Menjalankan

### Mode Interaktif:
```bash
python ai.py
```

### Langsung kirim pertanyaan:
```bash
python ai.py -t "Hai AI!" -es on
```

### Simpan otomatis ke file:
```bash
python ai.py -t "Apa kabar?" -es off -o hasil.json
```

### Bantuan:
```bash
python ai.py --help
```

---

## Struktur File

- `ai.py` â€” Skrip utama chatbot
- `user_config.json` â€” Tersimpan otomatis (nama dan preferensi espeak)
- `hasil.txt` / `hasil.json` â€” File output jika menyimpan percakapan

---

## API yang Digunakan

[Blackbox AI API](https://api.siputzx.my.id/api/ai/blackboxai-pro?content=)

Contoh response:
```json
{
  "status": true,
  "data": "Hello! How can I assist you today?"
}
```

---

## Lisensi

MIT License
