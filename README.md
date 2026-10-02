# 🎧 VoxenPlus — Advanced Synced Lyrics Editor

VoxenPlus is a **fast, lightweight, and no-install** tool for creating **highly synchronized lyrics** with support for **line-by-line, word-by-word, and syllable-by-syllable timing**. It builds upon the original Voxen editor with additional lyric formats, improved performance, an upgraded UI, and advanced vocal support.

It’s built as a **single HTML file**, so it runs entirely in your browser on **PC and mobile**, with no setup required.

Just drop in your **MP3**, paste your lyrics, and start syncing. Simple as that.

## ✨ What Makes VoxenPlus Different?

VoxenPlus adds a range of features designed for creating more detailed and expressive synced lyrics:

* **Syllable-synchronized lyrics** with automatic syllable splitting
* **Background vocal support**
* **Duet mode** for assigning lyrics to different vocalists
* **Word-level synchronization**
* **Improved UI and preview experience**
* **Reduced lag and improved performance**
* **Multiple LRC export formats**
* **Flexible lyric formatting for compatible music players**

---

## 🌐 Try It Online

If you don’t want to download the HTML file, you can use the web version instead:

🔗 **[VoxenPlus Online](https://VoxenPlus.vercel.app)**

<div style="display: flex; gap: 10px;">
<img width="700" height="438" alt="VoxenPlus Desktop Preview" src="https://github.com/user-attachments/assets/063db70e-ab1f-4200-a1ae-a6e54209de81" />
<img width="200" height="438" alt="VoxenPlus Mobile Preview" src="https://github.com/user-attachments/assets/ba57efdd-9b79-4778-992e-9abed45df163" />
</div>

---

## ✨ Features

* **Line-level lyric timing** for simple synchronized lyrics
* **Word-level lyric timing** for karaoke-style effects
* **Syllable-level synchronization** for extremely precise lyrics
* **Automatic syllable splitting** to speed up syllable syncing
* **Background vocal lyrics** for backing vocals, harmonies, ad-libs, and other secondary vocals
* **Duet mode** for assigning lyrics to different singers
* **Improved UI** for a smoother editing experience
* **Improved performance** with reduced lag during syncing and previewing
* Add, remove, or modify lyric lines
* **Runs fully in the browser**
* **Works locally** with no internet connection required after loading
* **Export to LRC**
* **Multiple export formats**
* **Import and export projects** as JSON
* **Reaction Offset** support for timing adjustments
* **Preview Mode** for testing your synced lyrics
* **Mobile support**

---

## 🛠️ Usage Guide

1. From the **left-side panel**, upload your **MP3** file.
2. Paste or enter the plain lyrics of your song.
3. Choose your preferred synchronization mode.
4. Sync your lyrics while listening to the song.
5. Preview your result and export it in your preferred LRC format.

### ▸ Line Mode

Syncs lyrics **line-by-line**.

```text
(mm:ss:xx) For you I'd bleed myself dry
```

### ▸ Word Mode

Syncs lyrics **word-by-word** for precise karaoke-style timing.

**Advanced format**:

```text
<for:ss.xx:ss.xx|you:ss.xx:ss.xx|I'd:ss.xx:ss.xx|bleed:ss.xx:ss.xx|myself:ss.xx:ss.xx|dry:ss.xx:ss.xx>
```

**Pro format**:

```text
[01:28.866]v1:<01:28.866>Your <01:29.565>skin, <01:31.332>oh <01:31.669>yeah, <01:32.017>your <01:32.338>skin, <01:32.702>and <01:33.122>bones<01:33.874>
```

### ▸ Background Vocals

VoxenPlus supports separately timed background vocals, allowing backing vocals and harmonies to be synchronized independently from the main lyrics.

```text
[bg:<01:33.778>Ooh-<01:36.594>oo-<01:37.947>ooh<01:39.035>]
```

### ▸ Syllable Mode

VoxenPlus can synchronize lyrics down to the **individual syllable**, allowing significantly more precise highlighting and karaoke effects.

The editor can also **automatically split words into syllables**, reducing the amount of manual work required when creating syllable-synced lyrics.

### ▸ Duet Mode

Duet Mode allows lyrics to be assigned to different vocalists, making it possible to create synchronized lyrics for songs with multiple singers.

Vocal parts can be separated while retaining precise word and syllable timing.

---

## 📤 Export Formats

VoxenPlus supports multiple LRC output formats for compatibility with different music players.

### Advanced

Designed for players that support advanced word-level LRC data.

```text
<for:ss.xx:ss.xx|you:ss.xx:ss.xx|I'd:ss.xx:ss.xx|bleed:ss.xx:ss.xx>
```

### Pro

The default format for many compatible music players.

```text
[01:28.866]v1:<01:28.866>Your <01:29.565>skin, <01:31.332>oh <01:31.669>yeah
```

Background vocals can be exported separately:

```text
[bg:<01:33.778>Ooh-<01:36.594>oo-<01:37.947>ooh<01:39.035>]
```

You can switch between supported export formats directly from the sidebar.

---

## ⌨️ Controls

* **Enter** — Sync the current word, syllable, or line
* **Left Arrow** — Seek 5 seconds backward
* **Right Arrow** — Seek 5 seconds forward

---

## 🎵 Music App Compatibility

VoxenPlus is designed to work with music players that support advanced LRC features.

| App                                                                               | Word-by-Word | BG Vocals | Syllable-by-Syllable | Duet Support |
| --------------------------------------------------------------------------------- | ------------ | --------- | -------------------- | ------------ |
| [Metrolist](https://github.com/mostafaalagamy/Metrolist)                          | ✅ Yes        | ✅ Yes     | ✅ Yes                | ✅ Yes        |
| [Gramophone](https://github.com/FoedusProgramme/Gramophone)                       | ✅ Yes        | ✅ Yes     | ✅ Yes                | ✅ Yes        |
| [Oto Music](https://play.google.com/store/apps/details?id=com.piyush.music&hl=en) | ✅ Yes        | ❌ No      | ✅ Yes                | ❌ Limited    |

Compatibility depends on the specific LRC features supported by each music player.

---

## 🎥 Demo

<table>
  <tr>
    <td align="center">
      <b>App Used: <a href="https://github.com/FoedusProgramme/Gramophone">Gramophone</a></b><br>
      <video 
        src="https://github.com/user-attachments/assets/70a79040-3e19-44d8-8c99-af0754a72df0" 
        controls 
        width="200" 
        height="150">
      </video>
    </td>
    <td align="center">
      <b>App Used: <a href="https://github.com/mostafaalagamy/Metrolist">Metrolist</a></b><br>
      <video 
        src="https://github.com/user-attachments/assets/f709faf8-92d8-4de0-995d-fc0000465591" 
        controls 
        width="200" 
        height="150">
      </video>
    </td>
  </tr>
</table>

---

## 🚀 Why VoxenPlus?

VoxenPlus takes the simplicity of Voxen and adds the tools needed to create **modern, highly detailed synced lyrics**.

Whether you only need basic line synchronization or want to create **word-, syllable-, background-vocal-, and duet-synchronized lyrics**, VoxenPlus is designed to keep the process fast and straightforward.

No installation. No complicated setup. Just open the HTML file, add your song, and start syncing.
