<div align="center">

# Nue

*It's revolutionary*

**Speak Tamil. Be heard in English.**
**And the other way around.**

Real-time voice translation, built into the call.

</div>

---

## One call. Two languages. No barrier.

Meena speaks Tamil. John speaks English.
They've never understood each other. Until now.

Meena talks. John hears English.
John replies. Meena hears Tamil.

That's it. That's Nue.

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
Meena  ──►  Listen  ─►  Understand  ─►  Translate  ─►  Speak  ──►  John
 Tamil                                                            English

Meena  ◄──  Speak  ◄─  Translate  ◄─  Understand  ◄─  Listen  ◄──  John
```

|  |  |
|---|---|
| **Listen** | Knows when you're speaking, and when you've finished. |
| **Understand** | Turns your speech into text. |
| **Translate** | Carries your meaning into the other language. |
| **Speak** | Says it out loud, only to the person who needs to hear it. |

### Why the pause matters

In Tamil, the verb comes last.

> நான் நாளைக்கு கடைக்கு **போவேன்**
> *I · tomorrow · to the shop · **will go***

Nue has to hear the whole thought before it can say it in English. So it waits for your pause, then speaks. That's how the languages work, not a limitation of the software.

---

## Designed around the conversation

- **You never hear yourself translated.** Only the other person does.
- **You always see what Nue heard.** If it's wrong, just say it again.
- **The live speaker always wins.** Start talking and Nue stops to listen.
- **Tanglish just works.** "Meeting-க்கு late-ஆ வருவேன்" is how people really talk.

---

## Under the hood

|  |  |
|---|---|
| **Calls** | WebRTC via [LiveKit](https://livekit.io) |
| **Translator** | A Python agent that joins the call as an invisible participant |
| **Speech → Text** | Tamil and English speech recognition |
| **Translation** | Context-aware, so names and meaning carry through |
| **Text → Speech** | Natural Tamil and English voices |
| **App** | Web first, then mobile |

```
nue/
├── apps/web/     The calling app
├── agent/        The translator
├── server/       Sign-in and call setup
└── infra/        Local development
```

---

## Roadmap

- [ ] **Prove it.** Tamil → English on recorded audio. Measure accuracy and speed.
- [ ] **Both ways.** English → Tamil, on a live call between two people.
- [ ] **See it.** Live subtitles, with the original voice softly underneath.
- [ ] **Any phone.** Call a Nue number from any phone, no app needed.
- [ ] **In your pocket.** iOS and Android.

---

<div align="center">

**Nue** · In development

*Language shouldn't decide who you can talk to.*

</div>
