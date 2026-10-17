# 🎧 VoxenPlus — Advanced Synced Lyrics & LRC Editor

**VoxenPlus** is a free, lightweight, browser-based **synced lyrics editor** for creating precise **LRC files**, karaoke lyrics, and word-by-word or syllable-by-syllable lyric timing.

It is designed for people who want more control than a basic LRC editor provides, with support for **line timing, word timing, syllable timing, background vocals, up to three singers, duet lyrics, customizable keyboard controls, undo and redo, and multiple synchronization modes**.

VoxenPlus runs directly in your browser on **PC, iPad and mobile** with no installation required.

**Load your song. Add your lyrics. Sync them. Export your LRC.**

> 🍴 **VoxenPlus is a fork of [Voxen](https://github.com/Raqhael-ux/Voxen-LRC-Editor) by [Raqhael-ux](https://github.com/Raqhael-ux)**, based on Voxen v9.2b. The original editor, its sync workflow and the `.vxn` project format come from Voxen. Please take a look at the original project too.

## 🌐 Try VoxenPlus Online

**[VoxenPlus Online](https://voxenplus.vercel.app)**

No download or installation is required.

Prefer to run it locally? VoxenPlus is a single HTML file: download `index.html` from this repository and open it in your browser.

---

<p align="center">
  <img src="screenshot.png" alt="VoxenPlus with four layers: Lead, Background, Singer 2 and Singer 3">
</p>

---

## ⭐ VoxenPlus vs. Original Voxen

VoxenPlus is a fork of the original [Voxen](https://github.com/Raqhael-ux/Voxen-LRC-Editor) synced lyrics editor by [Raqhael-ux](https://github.com/Raqhael-ux). It keeps what Voxen does well and builds on it with syllable timing, a separate layer for every vocal part, undo and redo, a converter between Pro, Advanced and an experimental Test format, and more.

| Feature                                                    |    VoxenPlus    | Original Voxen  |
| ---------------------------------------------------------- | :-------------: | :-------------: |
| Line-by-line lyric timing                                  |        ✅        |        ✅        |
| Word-by-word lyric timing                                  |        ✅        |        ✅        |
| Syllable-by-syllable timing                                |        ✅        |        ❌        |
| Automatic syllable splitting                               |        ✅        |        ❌        |
| Manual syllable editing                                    |        ✅        |        ❌        |
| Merge and split syllables                                  |        ✅        |        ❌        |
| Background vocals                                          | ✅ (own layer)   | ✅ (line type)   |
| Multiple singers                                           |  ✅ (up to 3)    |  ✅ (up to 3)    |
| Every singer on a separate layer, shown side by side       |        ✅        |        ❌        |
| Tap sync mode                                              |        ✅        |        ✅        |
| Hold sync mode                                             |        ✅        |        ✅        |
| Hybrid sync mode                                           |        ✅        |        ✅        |
| Customizable keyboard controls                             |        ✅        |        ✅        |
| Remembers your keys, interface style and syllable fixes    |        ✅        |        ❌        |
| Reaction offset                                            |        ✅        |        ✅        |
| Timestamp shifting                                         |        ✅        |        ✅        |
| Sort lyrics by timestamp                                   |        ✅        |        ✅        |
| Undo and redo                                              |        ✅        |        ❌        |
| Clear all timestamps                                       |        ✅        |        ❌        |
| Pro ⇄ Advanced LRC converter                               |        ✅        |        ❌        |
| Test format (experimental): export, convert and open       |        ✅        |        ❌        |
| `.vxn` project files                                       |        ✅        |        ✅        |
| Interface style                                            | Modern + Legacy | Classic only    |
| Browser-based                                              |        ✅        |        ✅        |
| PC support                                                 |        ✅        |        ✅        |
| Mobile support                                             |        ✅        |        ✅        |
| LRC import                                                 |        ✅        |        ✅        |
| LRC export                                                 |        ✅        |        ✅        |
| No installation required                                   |        ✅        |        ✅        |

The *Original Voxen* column describes Voxen v9.2b, the version VoxenPlus is based on. Feature availability can change as both projects are developed.

---

## ✨ Features

VoxenPlus is built for detailed synchronized lyrics and karaoke-style timing.

### 🎵 Precise lyric synchronization

Create lyrics with multiple levels of timing:

* **Line-by-line synchronization**
* **Word-by-word synchronization**
* **Syllable-by-syllable synchronization** *(beta)*
* Precise karaoke-style word highlighting
* Independent timing for different vocal layers

### 🔤 Automatic syllable splitting

VoxenPlus can automatically divide words into syllables to make detailed lyric synchronization faster.

Syllables are cut the way they are sung — **fee·ling**, **drea·ming**, **figh·ting** — and every syllable gets its own timestamp.

Its syllable system can use multiple sources, including:

* TeX hyphenation
* CMU Pronouncing Dictionary
* Datamuse
* Wiktionary
* Spelling-based fallback rules (these take over when you are offline)

Only single words are looked up, never your whole lyrics, and the answers are remembered in your browser.

Incorrect splits can be manually corrected, and corrections can be remembered for future use. With syllables on, press **X** (or double-click / double-tap a word) to split it by hand, or type `·` inside a word when you edit a line.

This makes VoxenPlus useful for creating **syllable-timed lyrics**, karaoke lyrics, and highly precise LRC files.

### 🎙️ Multiple singers and vocals

VoxenPlus gives every vocal part its own layer:

* **Lead** (Singer 1)
* **Singer 2** — optional, added with **+ Singer 2**
* **Singer 3** — optional, added with **+ Singer 3** once Singer 2 has its layer
* **Background** vocals

You can also paste lyrics for Singer 2, Singer 3 and the background in the **Session** tab before you create the editor.

Every layer is timed on its own, so different vocal parts can overlap. Work on one layer at a time (press **B** to switch) or see all of them side by side with **Show all**. Lines can be moved between layers, and removing a Singer 2 or Singer 3 layer simply moves its lines back into the Lead layer, so nothing is lost.

Background lines can back a specific singer (**Backs** in the line editor, or *Auto* to pick the line they overlap most). They are written right after the line they back, so music players give them that singer.

In the exported file the singers are written as `v1`, `v2` and `v1000`. If your player prefers `v3` for the third singer, change **Output → Third singer label**.

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

Every key can be rebound from the **Keys** section: click a key, then press the new one. Your keys are remembered between visits.

| Action                   | Key      |
| ------------------------ | -------- |
| Previous line            | `W`      |
| Next line                | `S`      |
| Previous word            | `A`      |
| Next word                | `D`      |
| Seek back 5 seconds      | `←`      |
| Seek forward 5 seconds   | `→`      |
| Play / pause             | `Space`  |
| Set timestamp            | `Enter`  |
| Switch layer             | `B`      |
| Add line below           | `C`      |
| Edit line                | `E`      |
| Singer 1                 | `1`      |
| Singer 2                 | `2`      |
| Singer 3                 | `3`      |
| Move line to other layer | `4`      |
| Delete line              | `Delete` |
| Toggle preview           | `V`      |
| Split word (syllables)   | `X`      |
| Sort by time             | `R`      |
| Undo                     | `Z`      |
| Redo                     | `Y`      |

Undo and redo also work with `Ctrl` / `⌘` + `Z` and `Ctrl` / `⌘` + `Shift` + `Z` (and `Ctrl` + `Y` on Windows and Linux). Other `Ctrl`, `⌘` and `Alt` shortcuts stay with the browser. On Apple keyboards the `delete` key (⌫) deletes a line.

### ↩️ Undo and redo

Mistakes are cheap. Taps, edits, deletions, imports, sorting, offsets, layer moves, syllable splitting and clearing are all kept in a history of up to 300 steps. Use the arrows in the top bar (and next to **TAP** on touch devices) or the keys above.

### 🧹 Timestamp tools

* **Offset** (top bar) shifts every timestamp later or earlier by a number of minutes, seconds and milliseconds.
* **Clear times** (top bar, also **Output → Timestamps → Clear all**) removes every line and word timestamp on every layer. Your lyrics, singers and syllable splits stay as they are, and you can undo it.
* **Sort** puts the lines in order of their timestamps.

### 🔁 Format converter (Pro ⇄ Advanced ⇄ Test)

Got an LRC file in one format and need another? Open **Convert** (top bar, **Output** tab, welcome screen or the export dialog), paste or open the file, pick **Pro**, **Advanced** or the experimental **Test** format, then copy or save the result. VoxenPlus recognises the format of what you paste. Your session is not touched unless you press **Open in editor**.

To export your current session in another format, change **Output → Format**.

### 🖥️ Two interface styles

VoxenPlus comes with a **Modern** purple interface and a **Legacy** interface that keeps the classic Voxen layout (in purple). Switch between them in **Sync settings (⚙) → Interface**, or open the site with `?ui=legacy` or `?ui=modern`. Your choice is remembered, and your work is kept when you switch.

---

## 📝 LRC Editing

VoxenPlus supports creating and editing synchronized lyrics in several formats. **Advanced** is the format for Metrolist; **Pro** is the default for most apps.

### Line timing

Advanced:

```text
[00:12.00]{agent:v1}Light up the sky
[00:15.50]{agent:v1}We sing it loud
```

Pro:

```text
[00:12.000]v1:<00:12.000>Light up the sky<00:15.500>
[00:15.500]v1:<00:15.500>We sing it loud<00:19.500>
```

### Word timing

Advanced — the word times (in seconds) go on the line below the lyric:

```text
[00:05.00]{agent:v1}Light up the sky
<Light:5:5.5|up:5.5:6|the:6:6.5|sky:6.5:6.9>
```

Pro:

```text
[00:05.000]v1:<00:05.000>Light <00:05.500>up <00:06.000>the <00:06.500>sky<00:06.900>
```

### Syllable timing

In Pro the syllables of a word are written with no space between them. In Advanced the lyric line stays whole and the syllables are listed on the timing line.

Pro:

```text
[00:12.000]v1:<00:12.000>Drea<00:12.400>ming <00:12.800>of <00:13.200>the <00:13.600>mor<00:14.000>ning<00:14.400>
```

Advanced:

```text
[00:12.00]{agent:v1}Dreaming of the morning
<Drea:12:12.4|ming:12.4:12.8|of:12.8:13.2|the:13.2:13.6|mor:13.6:14|ning:14:14.4>
```

### Singers and background vocals

Pro:

```text
[00:05.000]v1:<00:05.000>Light <00:05.500>up <00:06.000>the <00:06.500>sky<00:06.900>
[bg:<00:06.000>(ooh)<00:06.400>]
[00:07.000]v2:<00:07.000>Hold <00:07.500>the <00:08.000>line<00:08.400>
[00:09.000]v1000:<00:09.000>Together <00:09.500>now<00:09.900>
```

Advanced:

```text
[00:05.00]{agent:v1}Light up the sky
<Light:5:5.5|up:5.5:6|the:6:6.5|sky:6.5:6.9>
[00:06.00]{agent:v1}{bg}(ooh)
<(ooh):6:6.4>
[00:07.00]{agent:v2}Hold the line
<Hold:7:7.5|the:7.5:8|line:8:8.4>
[00:09.00]{agent:v1000}Together now
<Together:9:9.5|now:9.5:9.9>
```

These formats allow VoxenPlus to create detailed synchronized lyrics for compatible music players.

---

## 📤 LRC Import & Export

VoxenPlus can import existing LRC files (**Open LRC** on the welcome screen, or **Output → Files → Open / Load text**) and export finished synchronized lyrics.

Supported output formats include:

* **Advanced LRC**
* **Pro LRC**
* **Test** (experimental, see below)
* Background vocal timing
* Singer 1, 2 and 3
* Word-level timing
* Syllable-level timing

From the **Export** dialog you can preview the LRC, copy it to your clipboard, save it as a `.lrc` file, or save a `.vxn` project.

### 🧪 Test format (experimental)

**Test** is a third output format, for trying out a new lyric file layout. It is experimental and may change.

Pick it in **Output → Format**, in the **Export** dialog, or as the target in **Convert**. Save it with **Output → Files → Save .test** (or the **.test** button of the Export dialog). VoxenPlus opens Test files too (**Open**, **Load text**, **Convert → Open file**, or paste into **Edit / import**), also when the text was copied out of a web page or a chat with `&lt;` and `&gt;` in place of `<` and `>`, or with a blank line between every line.

A Test file has four sections. This one was written by VoxenPlus:

```text
[meta]
mlx_version=1.0
lyric_source=VoxenPlus
last_fetched=
[song]
title=Example Song
artist=Example Artist
songwriters=
[agents]
v1=person
v2=person
v1000=group
[lyrics]
[part:00:05.000~00:08.400]Verse
[00:05.000~00:06.900|v1]<00:05.000>Light <00:05.500>up <00:06.000>the <00:06.500>sky <00:06.900> [bg:<00:06.000>(ooh)<00:06.400>]
[00:07.000~00:08.400|v2]<00:07.000>Hold <00:07.500>the <00:08.000>line<00:08.400>
[part:00:09.000~00:10.200]Chorus
[00:09.000~00:10.200|v1000]<00:09.000>To<00:09.250>geth<00:09.500>er <00:09.600><00:09.900>now<00:10.200>
```

* `[meta]` – the format version, where the lyrics came from (VoxenPlus writes `VoxenPlus`; a file you open keeps its own source) and when they were fetched (left empty).
* `[song]` – title, artist and songwriters. Type them in under **Output → Format → Test**; without a title, the name of your audio file is used. **Convert** takes the title and artist from the `[ti:]` and `[ar:]` tags of an LRC file, or the title from the file name.
* `[agents]` – the singers that sing in the file: `v1`, `v2`, and the third singer under the name you chose in **Third singer label** (`v3`, written as a `person`, or `v1000`, written as a `group`).
* `[part:start~end]Name` – a song part (Verse, Chorus ...), from the start of its first line to the end of its last. Give a line a part in **Edit line → Song part**: the part starts at that line and runs until the next one, and the row shows its name. Pro and Advanced have no parts, so they leave them out.
* `[start~end|agent]` – one line, with when it starts and ends and who sings it. Every `<time>` is where the text after it starts and where the text before it ends. The syllables of a word follow each other without a space (`To<00:09.250>geth<00:09.500>er`), two tags with nothing between them are a pause, and the last tag ends the line. A line you only timed as a whole is written as plain text.
* `[bg:...]` – the background vocals of a line sit inside it, with their own times and in brackets.

Pro → Test → Pro gives you the Pro file back, and Advanced → Test → Advanced the Advanced file. Going from Test to Pro closes the pauses between words (Pro cannot keep them), and Test to Pro or Advanced leaves out the song parts and the song details.

---

## 💾 `.vxn` Project Files

VoxenPlus uses the `.vxn` project format for saving and loading projects.

Project files allow you to save your current lyrics, timing information, vocal layers (including Singer 2, Singer 3 and the third singer label), syllable splits, song parts, the song details of the Test format and other editing data so you can continue working later. The audio is not stored in the project, so load your song again when you reopen it.

Projects saved by the original Voxen open in VoxenPlus too. Save and load them from the **Media** tab.

---

## 🎨 Preview Mode

Preview your synchronized lyrics before exporting them.

Preview mode shows every layer side by side, and each word and syllable lights up as it is sung.

Preview settings include:

* Glow effects
* Fade-in effects (Custom or Auto)
* Custom fade duration
* Glow speed
* Smooth or Simple animation

This makes it easier to check whether your timing looks correct before using the finished LRC file.

---

## 🛠️ Editing Tools

VoxenPlus includes tools for:

* Adding lyric lines
* Editing lyric lines
* Deleting lines
* Moving lines between vocal layers
* Assigning singers
* Adding Singer 2, Singer 3 and background vocal layers
* Filtering the Lead layer by singer
* Sorting lyrics by timestamp
* Splitting words into syllables
* Merging syllables
* Shifting timestamps
* Clearing all timestamps
* Undoing and redoing changes
* Converting between Pro and Advanced LRC
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

Audio is loaded directly into the browser for synchronization. If your browser cannot play a file by itself, VoxenPlus converts it inside the browser. This needs a one-time download of about 10 MB, so you have to be online the first time (files over 700 MB cannot be converted this way).

---

## 📱 PC, iPad & Mobile

VoxenPlus is designed to work in modern browsers on desktop, tablet and mobile devices. The keyboard shortcuts are designed for desktop and for an iPad with a keyboard.

On touch screens:

* **TAP** sets the time of the highlighted word. In Hold mode, keep your finger down for as long as the word is sung.
* **Tap a word** to jump to it and make it the next one to time.
* **Long-press a line** to edit it.
* **Double-tap a word** to split it into syllables (when syllables are on).
* **Undo and redo** are the arrows next to TAP, or in the top bar.
* **Swipe up** on the bottom bar to open the tools.

Turn a phone sideways and the controls become a single row, so the lyrics keep their room. One layer shows at a time then; switch with the layer buttons at the top. On phones with a notch, everything stays clear of it.

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
| [Metrolist](https://github.com/MetrolistGroup/Metrolist)    |      ✅      |         ✅         |        ✅        |    ✅    |
| [Gramophone](https://github.com/FoedusProgramme/Gramophone) |      ✅      |         ✅         |        ✅        |    ✅    |
| Oto Music                                                   |      ✅      |         ❌         |        ✅        | Limited |

Compatibility depends on the LRC features supported by each music player. Players also differ in how they show a third singer, so the **Third singer label** (`v1000` or `v3`) can be switched in the **Output** tab.

---

## 🚀 How to Use VoxenPlus

1. Open **VoxenPlus Online**.
2. Load your song (**Media** tab).
3. Add or import your lyrics (**Session** tab, or **Open LRC**). Singer 2, Singer 3 and background lyrics are optional.
4. Choose your synchronization level: Line, Word, or Syllable (beta), then press **Create editor**.
5. Select your vocal layer or singer. Add **Singer 2** and **Singer 3** layers if you need them.
6. Choose Tap, Hold, or Hybrid synchronization.
7. Sync your lyrics while the song plays.
8. Fine-tune timestamps and syllables. Undo anything you do not like.
9. Preview the result.
10. Export your synchronized lyrics as LRC (Pro or Advanced).

---

## 🔍 Why VoxenPlus?

VoxenPlus is designed for users looking for a **free synced lyrics editor**, **LRC editor**, **karaoke lyrics editor**, or a more advanced alternative to a basic lyric timing tool.

It combines:

* Line-level lyric timing
* Word-level lyric timing
* Syllable-level lyric timing
* Automatic syllable splitting
* Background vocals
* Up to three singers, each on their own layer
* Duet support
* Custom keyboard shortcuts
* Undo and redo
* Pro ⇄ Advanced LRC converter
* Multiple sync modes
* LRC import and export
* `.vxn` project files
* Browser-based editing
* PC, iPad and mobile support

All in a lightweight browser application.

**No installation. No account. Just load your song and start syncing.**

---

## ❓ Frequently Asked Questions

### What is VoxenPlus?

VoxenPlus is a browser-based synchronized lyrics and LRC editor for creating line-, word-, and syllable-timed lyrics. It is a fork of Voxen by Raqhael-ux.

### Is VoxenPlus free?

Yes. VoxenPlus is available as a browser-based application without requiring an account or installation.

### Does VoxenPlus support LRC files?

Yes. VoxenPlus supports LRC importing and exporting, including detailed word-level and syllable-level timing.

### Can I convert between Pro, Advanced and Test?

Yes. Use **Convert** in the top bar to convert a file between Pro LRC, Advanced LRC and the experimental Test format, or change **Output → Format** to export your current session in another format.

### What is the Test format?

An experimental lyric file layout that holds the song details, the singers, song parts, word and syllable timing and the background vocals in one text file (see **Test format** above). It exists to try the layout out; Pro and Advanced are the formats music players read today.

### Can VoxenPlus create karaoke lyrics?

Yes. Word-level and syllable-level synchronization can be used to create precise karaoke-style lyric timing.

### Does VoxenPlus support syllable timing?

Yes. VoxenPlus supports individual syllable timestamps and includes automatic syllable splitting. Syllable sync is currently in beta.

### Does VoxenPlus support background vocals?

Yes. Background vocals can be placed on their own layer and synchronized independently from the lead lyrics.

### Does VoxenPlus support multiple singers?

Yes. VoxenPlus supports up to three singers: Singer 1 (the Lead layer), Singer 2 and Singer 3. Each has its own layer, so they can overlap, and the background vocals have a layer of their own too.

### Can I undo a mistake?

Yes. Press `Ctrl` / `⌘` + `Z` (or use the undo arrow) to undo and `Ctrl` / `⌘` + `Shift` + `Z` to redo. Even **Clear times** can be undone.

### Can I use VoxenPlus on mobile?

Yes. VoxenPlus is designed to work in modern mobile browsers as well as desktop browsers, and it has touch controls for tablets and phones.

### Does VoxenPlus need to be installed?

No. VoxenPlus runs directly in the browser.

### Does VoxenPlus work offline?

Mostly. VoxenPlus is a single HTML file, so you can save it and open it locally. The dictionary lookups for syllable splitting (spelling rules take over when you are offline) and the converter for audio formats your browser cannot play both need an internet connection.

### What is a `.vxn` file?

A `.vxn` file is VoxenPlus's project format for saving and loading synchronized lyric projects. It is the same project format Voxen uses.

### Is VoxenPlus an alternative to Voxen?

VoxenPlus is a fork of [Voxen](https://github.com/Raqhael-ux/Voxen-LRC-Editor) by Raqhael-ux, based on Voxen v9.2b. It is built around the same core concept of a lightweight browser-based synced lyrics editor, while adding syllable timing, separate layers for up to three singers and background vocals, undo and redo, a converter, and more. The original Voxen is still a great choice if you only need simple line- and word-level syncing.

---

## 🔗 Links

**VoxenPlus:** https://voxenplus.vercel.app

**GitHub:** https://github.com/AetherIncarnate/VoxenPlus/tree/main

**Original Voxen (by Raqhael-ux):** https://github.com/Raqhael-ux/Voxen-LRC-Editor

**Original Voxen online:** https://raqhael-ux.github.io/Voxen-LRC-Editor/

---

## 🙏 Credits

VoxenPlus is a fork of **[Voxen](https://github.com/Raqhael-ux/Voxen-LRC-Editor) by [Raqhael-ux](https://github.com/Raqhael-ux)**, based on Voxen v9.2b. The original editor, its sync workflow and the `.vxn` project format come from Voxen. Thank you for building it!

Syllable splitting uses TeX hyphenation patterns, the CMU Pronouncing Dictionary, Datamuse and Wiktionary.

---

## 📌 Keywords

VoxenPlus, Voxen fork, fork of Voxen, synced lyrics editor, synchronized lyrics editor, LRC editor, LRC file editor, karaoke lyrics editor, karaoke LRC editor, word synced lyrics, word-by-word lyrics, syllable synced lyrics, syllable timing, lyric synchronization, lyric timestamp editor, background vocals LRC, duet lyrics, multi-singer lyrics, three singers lyrics, Pro to Advanced LRC converter, lyrics format converter, Test lyric format, advanced LRC, Pro LRC, browser LRC editor, online lyrics editor, free lyrics editor, Voxen alternative.
