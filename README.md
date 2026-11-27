# Liora Tools — Free, Ad-Free Client-Side Web Utilities

Open-source reference patterns and lightweight client-side utilities powering [Liora Tools](https://lioratools.com) — zero-backend browser tools running 100% locally in browser memory across 6 languages.

## Live Localized Implementations
* **German Percentage Calculator:** [Prozentrechner](https://lioratools.com/de/prozentrechner)
* **Turkish Percentage Calculator:** [Yüzde hesaplama](https://lioratools.com/tr/yuzde-hesaplama)
* **Portuguese Percentage Calculator:** [Calculadora de porcentagem](https://lioratools.com/pt/calculadora-de-porcentagem)
* **Spanish Case Converter:** [Cambiar mayúsculas a minúsculas](https://lioratools.com/es/cambiar-mayusculas-a-minusculas)
* **Portuguese Coin Flipper:** [Cara ou coroa](https://lioratools.com/pt/cara-ou-coroa)

---

## 1. Deterministic Comma & Dot Number Parser

Standard `parseFloat()` fails in international applications due to varying decimal and thousands separators (e.g., `1.234,56` vs `1,234.56`). 

### Core Logic & JavaScript Implementation
The parser handles dual-separator prioritization (the last separator acts as the decimal point), single-separator thousands detection (3 trailing digits), and signed percentage delta calculations (`Math.abs(start)`). 

To view or copy the complete `parseLocaleNumber` JavaScript function, refer to the full source implementation.

---

## 2. Safe Auto-Resizing `<iframe>` Embeds

Embedded routes emit `liora-embed-height` postMessages validated against `event.source` to dynamically adjust frame heights safely without layout shifts. For the complete HTML/JS embed snippet, see the full repository documentation.

---

## 3. Cryptographically Fair Randomness

Decision tools like [Cara ou coroa](https://lioratools.com/pt/cara-ou-coroa) utilize `window.crypto.getRandomValues()` to generate unbiased outcomes directly in tab memory. The complete `getFairCoinFlip()` function can be found in the source code.

## License

MIT License — free to use, inspect, and embed.

