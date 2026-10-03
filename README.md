  # 🎧 VoxenPlus — Advanced Synced Lyrics & LRC Editor

**VoxenPlus** is a free, lightweight, browser-based **synced lyrics editor** for creating precise **LRC files**, karaoke lyrics, and word-by-word or syllable-by-syllable lyric timing.

It is designed for people who want more control than a basic LRC editor provides, with support for **line timing, word timing, syllable timing, background vocals, multiple singers, duet lyrics, customizable keyboard controls, and multiple synchronization modes**.

VoxenPlus runs directly in your browser on **PC and mobile** with no installation required.

**Load your song. Add your lyrics. Sync them. Export your LRC.**

## 🌐 Try VoxenPlus Online

**[VoxenPlus Online](https://voxenplus.vercel.app)**

No download or installation is required.

---

<p align="center">
  <img src="https://i.ibb.co/rgycjB9/IMG-2133.jpg" alt="VoxenPlus screenshot" width="800">
</p>

---

## ⭐ VoxenPlus vs. Original Voxen

VoxenPlus builds on the original Voxen synced lyrics editor with additional editing, synchronization, vocal-layer, and project features.

| Feature                        | VoxenPlus | Original Voxen |
| ------------------------------ | :-------: | :------------: |
| Line-by-line lyric timing      |     ✅     |        ✅       |
| Word-by-word lyric timing      |     ✅     |        ✅       |
| Syllable-by-syllable timing    |     ✅     |        ❌       |
| Automatic syllable splitting   |     ✅     |        ❌       |
| Manual syllable editing        |     ✅     |        ❌       |
| Background vocals              |     ✅     |        ❌       |
| Multiple singer layers         |     ✅     |        ❌       |
| Tap sync mode                  |     ✅     |        ✅       |
| Hold sync mode                 |     ✅     |        ✅       |
| Hybrid sync mode               |     ✅     |        ✅       |
| Customizable keyboard controls |     ✅     |        ❌       |
| Reaction offset                |     ✅     |        ✅       |
| Timestamp shifting             |     ✅     |        ❌       |
| Merge and split syllables      |     ✅     |        ❌       |
| Sort lyrics by timestamp       |     ✅     |        ❌       |
| `.vxn` project files           |     ✅     |        ✅       |
| Configurable themes            |     ✅     |      Limited    |
| Browser-based                  |     ✅     |        ✅       |
| PC support                     |     ✅     |        ✅       |
| Mobile support                 |     ✅     |        ✅       |
| LRC import                     |     ✅     |        ✅       |
| LRC export                     |     ✅     |        ✅       |
| No installation required       |     ✅     |        ✅       |

Feature availability can change as both projects are developed.

---

## ✨ Features

VoxenPlus is built for detailed synchronized lyrics and karaoke-style timing.

### 🎵 Precise lyric synchronization

Create lyrics with multiple levels of timing:

* **Line-by-line synchronization**
* **Word-by-word synchronization**
* **Syllable-by-syllable synchronization**
* Precise karaoke-style word highlighting
* Independent timing for different vocal layers

### 🔤 Automatic syllable splitting

VoxenPlus can automatically divide words into syllables to make detailed lyric synchronization faster.

Its syllable system can use multiple sources, including:

* TeX hyphenation
* CMU Pronouncing Dictionary
* Datamuse
* Wiktionary
* Spelling-based fallback rules

Incorrect splits can be manually corrected, and corrections can be remembered for future use.

This makes VoxenPlus useful for creating **syllable-timed lyrics**, karaoke lyrics, and highly precise LRC files.

### 🎙️ Multiple singers and vocals

VoxenPlus supports multiple vocal layers, including:

* Lead vocals
* Singer 2
* Background vocals

Different vocal parts can overlap and be synchronized independently.

This is useful for:

* Duets
* Harmonies
* Backing vocals
* Ad-libs
* Multiple vocalists
* Call-and-response lyrics

### ⏱️ Multiple synchronization modes

VoxenPlus provides three synchronization modes:

**Tap** — press the synchronization key to record timestamps.

**Hold** — use a held key for continuous timing control.

**Hybrid** — combines tap and hold behavior.

You can also use **Reaction Offset** to compensate for the delay between hearing a lyric and pressing a key.

### ⌨️ Custom keyboard controls

Keyboard shortcuts can be customized directly inside the editor.

Every key can be rebound from the **Keys** section.

| Action                   | Key      |
| ------------------------ | -------- |
| Previous line            | `W`      |
| Next line                | `S`      |
| Previous word            | `A`      |
| Next word                | `D`      |
| Seek backward            | `←`      |
| Seek forward             | `→`      |
| Play / pause             | `Space`  |
| Set timestamp            | `Enter`  |
| Switch layer             | `B`      |
| Add line                 | `C`      |
| Edit line                | `E`      |
| Singer 1                 | `1`      |
| Singer 2                 | `2`      |
| Move line between layers | `4`      |
| Delete line              | `Delete` |
| Preview                  | `V`      |
| Split syllables          | `X`      |
| Sort by timestamp        | `R`      |

---

## 📝 LRC Editing

VoxenPlus supports creating and editing synchronized lyrics in several formats.

### Line timing

```text
(mm:ss:xx) For you I'd bleed myself dry
```

### Word timing

```text
<for:ss.xx:ss.xx|you:ss.xx:ss.xx|I'd:ss.xx:ss.xx|bleed:ss.xx:ss.xx>
```

### Pro format

```text
[01:28.866]v1:<01:28.866>Your <01:29.565>skin, <01:31.332>oh <01:31.669>yeah
```

### Background vocals

```text
[bg:<01:33.778>Ooh-<01:36.594>oo-<01:37.947>ooh<01:39.035>]
```

These formats allow VoxenPlus to create detailed synchronized lyrics for compatible music players.

---

## 📤 LRC Import & Export

VoxenPlus can import existing LRC files and export finished synchronized lyrics.

Supported output formats include:

* **Advanced LRC**
* **Pro LRC**
* Background vocal timing
* Word-level timing
* Syllable-level timing

You can also copy generated LRC directly to your clipboard.

---

## 💾 `.vxn` Project Files

VoxenPlus uses the `.vxn` project format for saving and loading projects.

Project files allow you to save your current lyrics, timing information, vocal layers, and other editing data so you can continue working later.

---

## 🎨 Preview Mode

Preview your synchronized lyrics before exporting them.

Preview controls include:

* Glow effects
* Fade-in effects
* Custom fade duration
* Glow speed
* Layer switching
* Singer selection

This makes it easier to check whether your timing looks correct before using the finished LRC file.

---

## 🛠️ Editing Tools

VoxenPlus includes tools for:

* Adding lyric lines
* Editing lyric lines
* Deleting lines
* Moving lines between vocal layers
* Assigning singers
* Adding background vocals
* Sorting lyrics by timestamp
* Splitting words into syllables
* Merging syllables
* Shifting timestamps
* Adjusting reaction offset
* Previewing synchronized lyrics

---

## 🎵 Audio Support

VoxenPlus supports a wide range of common audio formats, including:

* MP3
* WAV
* FLAC
* M4A
* OGG
* WMA
* AIFF

Audio is loaded directly into the browser for synchronization.

---

## 📱 PC & Mobile

VoxenPlus is designed to work in modern browsers on both desktop and mobile devices.

It does not require:

* An installer
* A desktop application
* A mobile application
* An account

Open VoxenPlus, load your audio, and start editing.

---

## 🎶 Music Player Compatibility

VoxenPlus is designed for music players that support advanced LRC features.

| Music Player                                                | Word Timing | Background Vocals | Syllable Timing |   Duet  |
| ----------------------------------------------------------- | :---------: | :---------------: | :-------------: | :-----: |
| [Metrolist](https://github.com/mostafaalagamy/Metrolist)    |      ✅      |         ✅         |        ✅        |    ✅    |
| [Gramophone](https://github.com/FoedusProgramme/Gramophone) |      ✅      |         ✅         |        ✅        |    ✅    |
| Oto Music                                                   |      ✅      |         ❌         |        ✅        | Limited |

Compatibility depends on the LRC features supported by each music player.

---

## 🚀 How to Use VoxenPlus

1. Open **VoxenPlus Online**.
2. Load your song.
3. Add or import your lyrics.
4. Choose your synchronization level.
5. Select your vocal layer or singer.
6. Choose Tap, Hold, or Hybrid synchronization.
7. Sync your lyrics while the song plays.
8. Fine-tune timestamps and syllables.
9. Preview the result.
10. Export your synchronized lyrics as LRC.

---

## 🔍 Why VoxenPlus?

VoxenPlus is designed for users looking for a **free synced lyrics editor**, **LRC editor**, **karaoke lyrics editor**, or a more advanced alternative to a basic lyric timing tool.

It combines:

* Line-level lyric timing
* Word-level lyric timing
* Syllable-level lyric timing
* Automatic syllable splitting
* Background vocals
* Multiple singers
* Duet support
* Custom keyboard shortcuts
* Multiple sync modes
* LRC import and export
* `.vxn` project files
* Browser-based editing
* PC and mobile support

All in a lightweight browser application.

**No installation. No account. Just load your song and start syncing.**

---

## ❓ Frequently Asked Questions

### What is VoxenPlus?

VoxenPlus is a browser-based synchronized lyrics and LRC editor for creating line-, word-, and syllable-timed lyrics.

### Is VoxenPlus free?

Yes. VoxenPlus is available as a browser-based application without requiring an account or installation.

### Does VoxenPlus support LRC files?

Yes. VoxenPlus supports LRC importing and exporting, including detailed word-level and syllable-level timing.

### Can VoxenPlus create karaoke lyrics?

Yes. Word-level and syllable-level synchronization can be used to create precise karaoke-style lyric timing.

### Does VoxenPlus support syllable timing?

Yes. VoxenPlus supports individual syllable timestamps and includes automatic syllable splitting.

### Does VoxenPlus support background vocals?

Yes. Background vocals can be placed on their own layer and synchronized independently from the lead lyrics.

### Does VoxenPlus support multiple singers?

Yes. VoxenPlus supports multiple singer layers, including Singer 1 and Singer 2.

### Can I use VoxenPlus on mobile?

Yes. VoxenPlus is designed to work in modern mobile browsers as well as desktop browsers.

### Does VoxenPlus need to be installed?

No. VoxenPlus runs directly in the browser.

### What is a `.vxn` file?

A `.vxn` file is VoxenPlus's project format for saving and loading synchronized lyric projects.

### Is VoxenPlus an alternative to Voxen?

VoxenPlus is based around the same core concept of a lightweight browser-based synced lyrics editor, while adding additional synchronization, syllable, vocal-layer, editing, and project features.

---

## 🔗 Links

**VoxenPlus:** https://voxenplus.vercel.app

**GitHub:** https://github.com/mikerotchburnes103/VoxenPlus

---

## 📌 Keywords

VoxenPlus, synced lyrics editor, synchronized lyrics editor, LRC editor, LRC file editor, karaoke lyrics editor, karaoke LRC editor, word synced lyrics, word-by-word lyrics, syllable synced lyrics, syllable timing, lyric synchronization, lyric timestamp editor, background vocals LRC, duet lyrics, multi-singer lyrics, advanced LRC, Pro LRC, browser LRC editor, online lyrics editor, free lyrics editor, Voxen alternative.
