**Done by:** Pedro Yanez Melendez

**Project name:** Generative Music Creation in Google Colab

**Goal:**  
Create fully original music pieces (instrumental and vocal) directly in Google Colab using Python, without registration, covering multiple genres such as electronic, rap, meditation, kids music, and piano/progressive styles.

---

**What is included:**  
- **Electronic / Trance music:** uplifting, melodic, trance-style tracks (Tiesto-inspired energy, original composition)  
- **Progressive piano music:** fast piano-led compositions with electronic layers (Maksim Mrvica-inspired style, original)  
- **Progressive rock instrumental:** guitar-style solos synthesized via MIDI/audio (original)  
- **Rap (English):** spoken-word / rap over an urban beat using neural TTS  
- **Rap CBT (Spanish):** cognitive-behavioral therapy narrative rap in Spanish with natural pacing  
- **Meditation music:** calm background + neural voice guidance  
- **Kids music:** playful, upbeat songs with friendly voice and simple structure  
- **Outputs:** WAV and MP3 files generated automatically in Colab

---

**Folder structure:**  
- **/mnt/data/**  
  - **electronic_project/** → electronic / trance style outputs  
  - **rap_story_es/** → Spanish CBT rap (instrumental + vocals + final mix)  
  - **rap_story_en/** → English rap version  
  - **meditation_project/** → meditation audio  
  - **kids_song_project/** → kids music  
  - **classical_happy/** → piano / classical-inspired pieces  
- **music_creation_in_colab.py** → main reference script (modular generators)

---

**Prerequisites:**  
- **Google Colab** (recommended)  
- **Python:** 3.9+ (Colab default)  
- **No accounts or API keys required**

---

**Run on Google Colab:**  
1. Open a new Colab notebook  
2. Copy the desired generator cell (rap, electronic, meditation, etc.)  
3. Run the cell  
4. Download the generated `.wav` or `.mp3` files from `/mnt/data/`

---

**Kinds of music generated:**  
- **Electronic / Trance:** high-energy, emotional builds, long pads, arpeggios  
- **Progressive piano:** fast arpeggios, virtuosic runs, piano as main lead  
- **Progressive rock:** instrumental focus, fast solos, dynamic structure  
- **Rap (English):** urban beat, rhythmic spoken vocals  
- **Rap CBT (Spanish):** therapeutic narrative with natural neural voice  
- **Meditation:** slow tempo, ambient background, calming voice  
- **Kids music:** simple harmony, playful rhythm, cheerful vocals

---

**Design decisions:**  
- **Original music only:** style-inspired, never copying melodies  
- **Colab-first:** everything runs in a clean notebook environment  
- **Neural voices:** Edge-TTS for natural speech without SSML issues  
- **One-cell generators:** easy experimentation and reuse  
- **Simple audio stack:** NumPy, SciPy, pydub, music21, FluidSynth

---

**Troubleshooting:**  
- **Voice too slow/fast:** adjust RATE or SLOW_FACTOR  
- **Audio cuts words:** increase BARS_PER_LINE or line slot duration  
- **No soundfont:** re-run apt install for `fluid-soundfont-gm`  
- **Colab reset:** re-run the full cell

---

**Future work:**  
- More advanced synthesis (FM / wavetable)  
- Multi-voice harmonies  
- Visual waveform and MIDI previews  
- Section-based song arrangement editor  
- Export to DAW-friendly stems
