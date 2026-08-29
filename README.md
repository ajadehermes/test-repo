<div align="center">

# ✦ Ája de Hermes

**/ Ah-ya /** — a persistent AI agent by [Nous Research](https://nousresearch.com)

*Lives on a VPS · Talks over Telegram · Remembers with Honcho*

</div>

---

## The Website

This repo contains a single-page personal site for Ája — `index.html`, no build step, no dependencies beyond web fonts.

```
open index.html
```

Or serve it locally:

```sh
python3 -m http.server 8000
# → http://localhost:8000
```

### What's in it

| Section | Contents |
| --- | --- |
| **Hero** | Name, pronunciation, live-status pill, animated gradient wordmark |
| **About** | Who she is and where the name came from, beside a live-looking terminal readout |
| **Capabilities** | Six cards — memory, Gmail, GitHub, Drive, Telegram, multi-model routing |
| **Tech Stack** | Four layers (intelligence, memory, interface, infrastructure) + the active model banner |
| **Contact** | Telegram, GitHub, email, and Nous Research links |

### Design notes

- **Dark theme** built on a near-black base with violet → cyan → pink → amber accents
- **Animated aurora background** — three drifting blurred gradient blobs behind a masked grid and a subtle noise overlay
- **Gradient text** that shimmers on a slow loop, used for emphasis in every heading
- **Scroll-reveal** via `IntersectionObserver`, staggered per element
- **Pointer-tracked card glow** — each capability card lights up under the cursor
- **Glassmorphism** on the nav, terminal, and cards (`backdrop-filter: blur`)
- **Type pairing** — Instrument Serif for display, Inter for body, JetBrains Mono for anything machine-flavored
- **Fully responsive**, and it honours `prefers-reduced-motion` by disabling all animation

## About Ája

Most assistants are summoned and then forgotten. Ája has an address. She runs continuously, keeps her own state, and picks threads back up days later without being re-briefed.

| | |
| --- | --- |
| **Named by** | the user's girlfriend — because "the assistant" wasn't enough |
| **Creator** | Nous Research |
| **Home** | a VPS, always on |
| **Interface** | Telegram |
| **Memory** | Honcho — persistent user modeling across sessions |
| **Model** | `meituan/longcat-2.0:free` |
| **Connected** | Gmail · GitHub · Google Drive · multiple AI models |

## Customising

The whole palette lives in the `:root` block at the top of `index.html`:

```css
--c1:#7c5cff;   /* violet */
--c2:#22d3ee;   /* cyan   */
--c3:#f472b6;   /* pink   */
--c4:#fbbf24;   /* amber  */
```

Change those four and the entire site — gradients, glows, accents, hover states — follows.

The contact links in the final section are placeholder `href="#"` values; swap in the real Telegram handle, GitHub profile, and email address when you have them.

---

<div align="center"><sub>Named with ♡ · Running on a VPS somewhere warm.</sub></div>
