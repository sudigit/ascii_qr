# ASCII Art: scan, snap, save

Visitors scan a QR code, take a selfie (or pick a photo) and get their ASCII art, which they can save.
Everything runs **in the visitor's browser**: no server, no app, and photos never leave their phone.

| File | What it is |
|---|---|
| `index.html` | the phone page: take/choose photo → ASCII art → save / share |
| `qr.html` | big QR code pointing to `index.html`. Open it on the laptop screen or print it |

## Deploy on GitHub Pages (free)

1. On github.com: **New repository** → name it e.g. `ascii-art` → **Public** → Create.
2. **Add file → Upload files** → drag in `index.html`, `qr.html`, `README.md` → **Commit changes**.
3. **Settings → Pages** → Source: **Deploy from a branch** → Branch: **main**, folder **/ (root)** → **Save**.
4. Wait 1–2 minutes. Your links:
   - page: `https://<your-username>.github.io/ascii-art/`
   - QR:   `https://<your-username>.github.io/ascii-art/qr.html`
5. Open the QR link on the event laptop (or press Ctrl+P to print it). Scan it with your phone to test.

## Test locally (optional)
```
python -m http.server 8000
```
then open http://localhost:8000 in a browser.
