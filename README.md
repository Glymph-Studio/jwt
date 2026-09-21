# jwt — Glymph Studio

> Terminal-grade JWT decoder. Live, private, zero dependencies.

**Live:** `jwt.glymph.vercel.app` (or `glymph.vercel.app/jwt`)  
**Built by:** [@Yash-Tripath1](https://github.com/Yash-Tripath1) for [Glymph Studio](https://github.com/glymph-studio)

Decoded entirely in your browser. Nothing is sent anywhere. 🔒

![black terminal](https://img.shields.io/badge/background-%230a0a0a-black) ![vanilla JS](https://img.shields.io/badge/vanilla-JS-yellow) ![single file](https://img.shields.io/badge/single-HTML-file)

### Preview
Paste any JWT → instantly see header / payload / signature with color highlighting:
- **header** `#ffffff` white
- **payload** `#9a9a9a` gray  
- **signature** `#4a4a4a` dim

### Why this beats jwt.io / jwt.ms / token.dev
- No tracking, no cookies, no localStorage, single 31KB HTML
- Input highlights 3 parts live as you type (they don't)
- Plain-English claim explanations BELOW value + live `VALID in 2h` / `EXPIRED 3d ago` badges
- Full UI shifts to red-tinted state on expired — unmissable
- Terminal aesthetic: #0a0a0a, JetBrains Mono, thin lines only, only blink animation
- Bearer prefix auto-strip, drag & drop, URL hash share, timeline visualization, RAW+JSON copy

### Features
- [x] Live decode, no button
- [x] Color-highlighted textarea (overlay trick)
- [x] Formatted JSON for header/payload
- [x] Copy JSON + Copy RAW per section
- [x] Standard claims explained: `exp`, `iat`, `nbf`, `sub`, `iss`, `aud`, `jti`, `azp` + more
- [x] Live exp countdown (1s interval)
- [x] Red-tint expired state + yellow nbf future warning
- [x] ALG prominently with `Signature cannot be verified client-side`
- [x] `Token is malformed` state
- [x] Timeline `iat → now → exp` with progress %
- [x] Stats: token length, header/payload/sig sizes
- [x] Bearer + Authorization header auto-strip, whitespace handling
- [x] Supports `alg:none` with empty signature
- [x] Paste button, Clear (Esc), drag & drop, URL hash share
- [x] Mobile responsive
- [x] Sticky privacy badge

### Tech
- Single `index.html`
- Vanilla JS, no deps, no backend
- JetBrains Mono via Google Fonts
- Works offline

### Run locally
```bash
# just open
open index.html
# or serve
npx serve .
```

### Deploy to Vercel (Glymph org)
1. Create repo under `glymph-studio` org → `jwt` (public)
2. Push:
```bash
git clone https://github.com/glymph-studio/jwt.git
cd jwt
git config user.name "Yash-Tripath1"
git config user.email "tripathiyash382@gmail.com"
# copy files
git add .
git commit -m "feat: jwt terminal decoder"
git push origin main
```
3. Vercel → Import `glymph-studio/jwt` → Deploy → Add domain `jwt.glymph.vercel.app`

Contributions will show on both your profile and the org.

### Credits
Built by [@Yash-Tripath1](https://github.com/Yash-Tripath1)  
Part of [Glymph Studio](https://glymph.vercel.app) — indie studio building tools fast, from scratch.

### License
MIT — see LICENSE
