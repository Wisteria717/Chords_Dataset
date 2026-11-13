# Chords_Dataset
Dataset containing wav files at 120 bpm (4/4) and chords (triads) major and minor being played for 4 notes. 
Starting Chord: C then C# and so on till B two octaves higher therefore, 24 chords.

Major and minor chords:
Piano, Electric_Guitar, Acoutic_Guitar, Accordian: C3-B4 (24 roots)
Oragn, Synth_Bass: C2-B3 (24 roots)

Piano, Metal_Guitar, Organ: C3-B4 (1st and 2nd Inversions)

## Update: Batches

The WAV files are now split into two batches, identified by a prefix in the filename.

**FirstBatch** – the original MIDI-generated recordings described above, now renamed with a `FirstBatch - ` prefix (e.g. `FirstBatch - MajorC3-B4_Piano.wav`). Each file plays all 24 chords in chromatic order.

**SecondBatch** – real guitar recordings, named `SecondBatch - <Key><maj|min>Guitar.wav` (e.g. `SecondBatch - F#minGuitar.wav`). 
### Recording Session Summary

* **Tempo & Timing:** 120 BPM (2 beats per second / 0.5 seconds per beat)
* **Duration per Chord:** 4 beats (1 bar in 4/4 time) = **2 seconds**
* **Duration per Track:** 8 chords (32 beats / 8 bars) = **16 seconds**
* **Total Tracks Recorded:** 12 audio files
* **Total Audio Captured:** 96 chord instances (384 beats) = **3 minutes 12 seconds** of raw playing

---

### Exact Chord Tally Across All 12 Tracks

Because you looped each 4-chord sequence twice per track, every progression yielded **2 recordings** of its chords right away—meaning you actually captured **4 recordings of most chords**, and **at least 2 recordings of every single one of the 24 chords**:

| Chord Type | 2 Recordings Captured | 4 Recordings Captured | 6 Recordings Captured |
| --- | --- | --- | --- |
| **Major Chords (12)** | C, D, E, F#, Ab, Bb | Db, Eb, F, G, A, B | — |
| **Minor Chords (12)** | Cm, Dm, Em, F#m, G#m, Bbm | Bm, C#m, D#m, Gm | Fm, Am |

---

### Track-by-Track Log (16 Seconds Each)

**Major-Key Loops (I – IV – V – vi × 2)**

1. **Track 1 (C Major):** `C – F – G – Am – C – F – G – Am`
2. **Track 2 (D Major):** `D – G – A – Bm – D – G – A – Bm`
3. **Track 3 (E Major):** `E – A – B – C#m – E – A – B – C#m`
4. **Track 4 (F# Major):** `F# – B – C# – D#m – F# – B – C# – D#m`
5. **Track 5 (Ab Major):** `Ab – Db – Eb – Fm – Ab – Db – Eb – Fm`
6. **Track 6 (Bb Major):** `Bb – Eb – F – Gm – Bb – Eb – F – Gm`

**Minor-Key Loops (i – iv – v – VI × 2)**
7. **Track 7 (C Minor):** `Cm – Fm – Gm – Ab – Cm – Fm – Gm – Ab`
8. **Track 8 (D Minor):** `Dm – Gm – Am – Bb – Dm – Gm – Am – Bb`
9. **Track 9 (E Minor):** `Em – Am – Bm – C – Em – Am – Bm – C`
10. **Track 10 (F# Minor):** `F#m – Bm – C#m – D – F#m – Bm – C#m – D`
11. **Track 11 (G# Minor):** `G#m – C#m – D#m – E – G#m – C#m – D#m – E`
12. **Track 12 (Bb Minor):** `Bbm – Ebm – Fm – Gb – Bbm – Ebm – Fm – Gb`

If you are slicing these into a sample pack or dataset, every chord slice is cleanly quantized to **2.0 seconds (44,100 or 48,000 samples × 2)** starting right on the downbeat of every bar.