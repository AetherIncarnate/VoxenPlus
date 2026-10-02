# 🎧 VoxenPlus — Advanced Synced Lyrics Editor

VoxenPlus is a **fast, lightweight, and no-install** tool for creating highly synchronized lyrics with support for **line-by-line, word-by-word, and syllable-by-syllable timing**.

VoxenPlus expands on the original Voxen editor with **background vocals, multiple singer layers, automatic syllable splitting, customizable controls, improved syncing modes, and a smoother editing experience**.

It runs directly in your browser on **PC and mobile**, with no installation required.

Just load your song, add your lyrics, and start syncing.

## 🌐 Try It Online

Use VoxenPlus directly in your browser:

🔗 **[VoxenPlus Online](https://voxenplus.vercel.app)**

---

## ✨ Features

* **Line-by-line synchronization**
* **Word-by-word synchronization**
* **Syllable-by-syllable synchronization**
* **Automatic syllable splitting**
* **Background vocal support**
* **Multiple singer layers**
* **Duet support**
* **Third singer support**
* **Independent timing for each vocal layer**
* **Tap, Hold, and Hybrid syncing modes**
* **Customizable keyboard controls**
* **Reaction offset** for compensating for tapping/reaction delay
* **Preview mode** with configurable visual effects
* **Fade-in and glow controls**
* **Shift all timestamps** to move synchronized lyrics forward or backward
* **Import LRC files**
* **Export LRC files**
* **Import and export `.vxn` project files**
* **Copy generated LRC directly to the clipboard**
* **Add, edit, move, sort, and delete lyric lines**
* **Works locally in the browser**
* **Supports a wide range of audio formats**
* **Improved performance and reduced lag**

---

## 🎵 Audio Support

VoxenPlus supports a wide range of audio formats, including:

* MP3
* WAV
* FLAC
* M4A
* OGG
* WMA
* AIFF
* and more

Simply load your audio file into VoxenPlus and begin syncing.

---

## 🛠️ Usage Guide

1. Load your song using the **Audio Source** section.
2. Add your lead lyrics.
3. Optionally add lyrics for **Singer 2** and **Background Vocals**.
4. Choose your synchronization mode.
5. Create the editor.
6. Sync your lyrics while the song plays.
7. Preview your result.
8. Export your finished lyrics as an LRC file.

---

## 🎤 Vocal Layers

VoxenPlus allows different vocal parts to exist on separate layers.

### Lead

The primary lyrics of the song.

### Singer 2

Singer 2 has its own track and can be timed independently from the lead vocalist, allowing the two singers to overlap.

### Singer 3

A third singer layer is also available, with a customizable singer label.

### Background Vocals

Background vocals have their own layer and can overlap the lead lyrics independently.

This makes VoxenPlus suitable for songs containing **duets, harmonies, backing vocals, ad-libs, and multiple vocalists**.

---

## ⏱️ Sync Modes

VoxenPlus supports three ways of reading the synchronization key:

### Tap

Each press records a timestamp.

### Hold

Timing can be controlled by holding the synchronization key.

### Hybrid

Combines tap and hold behavior for more flexible synchronization.

You can also adjust the **Reaction Offset** to compensate for your reaction time. A negative offset can be used when your taps consistently occur slightly after the intended timing.

---

## 📝 Sync Levels

### ▸ Line Mode

Sync lyrics line-by-line.

```text
(mm:ss:xx) For you I'd bleed myself dry
```

### ▸ Word Mode

Synchronize individual words for precise karaoke-style highlighting.

**Advanced format:**

```text
<for:ss.xx:ss.xx|you:ss.xx:ss.xx|I'd:ss.xx:ss.xx|bleed:ss.xx:ss.xx|myself:ss.xx:ss.xx|dry:ss.xx:ss.xx>
```

**Pro format:**

```text
[01:28.866]v1:<01:28.866>Your <01:29.565>skin, <01:31.332>oh <01:31.669>yeah, <01:32.017>your <01:32.338>skin, <01:32.702>and <01:33.122>bones<01:33.874>
```

### ▸ Syllable Mode

VoxenPlus can synchronize individual syllables rather than entire words.

For example:

```text
fee·ling
beau·ti·ful
drea·ming
figh·ting
```

Each syllable can receive its own timestamp, allowing extremely precise lyric synchronization.

---

## 🔤 Automatic Syllable Splitting

VoxenPlus includes a syllable splitting system designed to automatically break words into syllables.

The system can use multiple sources to determine syllable boundaries, including:

* TeX hyphenation patterns
* CMU Pronouncing Dictionary
* Datamuse
* Wiktionary
* Spelling-based rules when offline

Individual words can also be corrected manually when automatic splitting isn't correct.

VoxenPlus can remember manual corrections and reuse them for the same word.

Only individual words are sent to online dictionaries rather than entire lyric passages, and dictionary results can be cached locally in the browser.

---

## 🎙️ Background Vocals

Background vocals can be synchronized independently from the main lyrics.

For example:

```text
[bg:<01:33.778>Ooh-<01:36.594>oo-<01:37.947>ooh<01:39.035>]
```

Background lines can overlap the lead lyrics and are exported alongside the line they back so compatible music players can associate them with the appropriate singer.

---

## 📤 Export

VoxenPlus supports multiple output formats.

### Advanced

Designed for music players that support advanced word-level LRC data.

```text
<for:ss.xx:ss.xx|you:ss.xx:ss.xx|I'd:ss.xx:ss.xx|bleed:ss.xx:ss.xx>
```

### Pro

Designed for broad compatibility with players supporting detailed LRC timing.

```text
[01:28.866]v1:<01:28.866>Your <01:29.565>skin, <01:31.332>oh <01:31.669>yeah
```

Background vocals can be included as their own lines:

```text
[bg:<01:33.778>Ooh-<01:36.594>oo-<01:37.947>ooh<01:39.035>]
```

You can switch between **Advanced** and **Pro** formats from the Output section.

---

## 💾 Project Files

VoxenPlus supports its own **`.vxn` project format**.

Projects can be saved and loaded so you can continue editing your work later without having to recreate your synchronization data.

You can also import existing LRC files into VoxenPlus.

---

## 🎨 Preview

VoxenPlus includes a preview system for checking how your synchronized lyrics behave.

Preview settings include:

* Preview glow
* Fade-in mode
* Custom fade duration
* Glow speed
* Layer switching
* Singer selection

This makes it easier to check your timing before exporting.

---

## ⌨️ Customizable Controls

Keyboard controls can be rebound directly inside VoxenPlus.

Default controls include:

| Action                     | Default Key |
| -------------------------- | ----------- |
| Previous line              | `W`         |
| Next line                  | `S`         |
| Previous word              | `A`         |
| Next word                  | `D`         |
| Seek back 5 seconds        | `←`         |
| Seek forward 5 seconds     | `→`         |
| Play / pause               | `Space`     |
| Set timestamp              | `Enter`     |
| Switch layer               | `B`         |
| Add line below             | `C`         |
| Edit line                  | `E`         |
| Set Singer 1               | `1`         |
| Set Singer 2               | `2`         |
| Set Singer 3               | `3`         |
| Move line to another layer | `4`         |
| Delete line                | `Delete`    |
| Toggle preview             | `V`         |
| Split word into syllables  | `X`         |
| Sort by time               | `R`         |

Every key can be rebound from the **Keys** section.

---

## 🎛️ Editing Tools

VoxenPlus provides tools for:

* Adding lines
* Editing lines
* Removing lines
* Moving lines between vocal layers
* Assigning singers
* Assigning background vocals
* Sorting lyrics by timestamp
* Splitting words into syllables
* Merging syllables
* Shifting all timestamps
* Adjusting reaction offset
* Previewing the final result

---

## 🎵 Music App Compatibility

VoxenPlus is designed for music players that support advanced LRC features.

| App                                                                               | Word-by-Word | BG Vocals | Syllable-by-Syllable | Duet Support |
| --------------------------------------------------------------------------------- | ------------ | --------- | -------------------- | ------------ |
| [Metrolist](https://github.com/mostafaalagamy/Metrolist)                          | ✅ Yes        | ✅ Yes     | ✅ Yes                | ✅ Yes        |
| [Gramophone](https://github.com/FoedusProgramme/Gramophone)                       | ✅ Yes        | ✅ Yes     | ✅ Yes                | ✅ Yes        |
| [Oto Music](https://play.google.com/store/apps/details?id=com.piyush.music&hl=en) | ✅ Yes        | ❌ No      | ✅ Yes                | ❌ Limited    |

Compatibility depends on which LRC features each music player supports.

---

## 🚀 Why VoxenPlus?

VoxenPlus takes the simplicity of the original Voxen editor and expands it into a more complete synchronized-lyrics editor.

Whether you want simple line timing, precise word synchronization, **syllable-level karaoke timing**, **background vocals**, or **multiple singers**, VoxenPlus provides the tools to build it.

It's lightweight, browser-based, and designed to keep the syncing process fast without requiring a complicated setup.

**No installation. No account. Just load your song and start syncing.**
