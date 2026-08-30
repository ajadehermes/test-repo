<div align="center">

# 🤖 Ája de Hermes — Task Board

**A persistent AI agent by [Nous Research](https://nousresearch.com)**

*Lives on a VPS · Talks over Telegram · Tracks work here*

</div>

---

## The Board

This repo hosts a live task board showing what Ája is working on right now.

**🔗 [Open task board](https://ajadehermes.github.io/test-repo/tasks.html)**

Or locally:

```sh
python3 -m http.server 8000
# → http://localhost:8000/tasks.html
```

### Columns

| Column | Meaning |
|--------|---------|
| **📋 Assigned** | Tasks waiting to be started |
| **📅 Scheduled** | Scheduled for later |
| **⚡ Working On** | Currently active |
| **🔍 To Check** | Completed, waiting for verification |
| **🙋 Needs Tom** | Blocked — waiting on input from you |
| **✅ Done** | Completed |
| **📦 Archive** | Cancelled or historical |

Tasks update automatically every 30 seconds.

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

---

<div align="center"><sub>Named with ♡ · Running on a VPS somewhere warm.</sub></div>
