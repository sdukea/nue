<div align="center">

# Nue

Real-time voice translation for calls, in any language.

</div>

---

## What it does

Two people on a call. Each speaks their own language.

You talk in yours. They hear you in theirs.
They reply in theirs. You hear them in yours.

Tamil and English. Japanese and Spanish. Hindi and French.
Any two languages, on one call.

---

## How it feels

It's like having an interpreter on the line. One who never gets tired.

**Speak naturally.** Say a sentence or two, then pause.
**Nue listens.** Your words appear on screen as you say them.
**They hear you.** In their language, about a second and a half later.

You'll still hear the other person's real voice, softly in the background. Their tone, their laugh, their warmth come through too.

---

## How it works

A call is two streams of sound, one each way.
Nue puts a translator in each stream.

```
You   ──►  Listen  ─►  Understand  ─►  Translate  ─►  Speak  ──►  Them
yours                                                            theirs

You   ◄──  Speak  ◄─  Translate  ◄─  Understand  ◄─  Listen  ◄──  Them
```

|  |  |
|---|---|
| **Listen** | Knows when you're speaking, and when you've finished. |
| **Understand** | Turns your speech into text. |
| **Translate** | Carries your meaning into the other language. |
| **Speak** | Says it out loud, only to the person who needs to hear it. |

Each person picks their language when they join. Nue always knows who speaks what.

### Why the pause matters

Languages don't share the same word order. Tamil, Hindi, Japanese, Korean and Turkish put the verb last.

> நான் நாளைக்கு கடைக்கு **போவேன்** · *Tamil*
> *I · tomorrow · to the shop · **will go***

English needs "will go" near the start, so Nue has to hear the whole thought first. It waits for your pause, then speaks. That's how the languages work, not a limitation of the software.

---

## Designed around the conversation

- **You never hear yourself translated.** Only the other person does.
- **You always see what Nue heard.** If it's wrong, just say it again.
- **The live speaker always wins.** Start talking and Nue stops to listen.
- **Mixed languages just work.** Tanglish, Hinglish, Spanglish: how people really talk.

---

## Under the hood

|  |  |
|---|---|
| **Calls** | WebRTC via [LiveKit](https://livekit.io) |
| **Translator** | A Python agent that joins the call as an invisible participant |
| **Speech → Text** | Speech recognition for each caller's language |
| **Translation** | Context-aware, so names and meaning carry through |
| **Text → Speech** | Natural voices in each caller's language |
| **App** | Web first, then mobile |

Each step can use a different provider for each language. Nue picks whichever handles that language best.

```
nue/
├── apps/web/     The calling app
├── agent/        The translator
├── server/       Sign-in and call setup
└── infra/        Local development
```

---

## Roadmap

- [ ] **Prove it.** One language pair on recorded audio, starting with Tamil → English. Measure accuracy and speed.
- [ ] **Both ways.** Live two-way translation on a call between two people.
- [ ] **See it.** Live subtitles, with the original voice softly underneath.
- [ ] **Every language.** Add languages one by one, each tested for accuracy and speed.
- [ ] **Any phone.** Call a Nue number from any phone, no app needed.
- [ ] **In your pocket.** iOS and Android.

---

<div align="center">

**Nue** · In development

</div>
