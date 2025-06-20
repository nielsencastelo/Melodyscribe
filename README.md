# Melodyscribe 🎼🤖

**Status: In development.** 🚧

Melodyscribe is an AI-based system for automatic transcription of songs (WAV, MP3) into sheet music in PDF format, with support for multiple instruments and voice.

## 🎯 Goal

To build a collaborative tool based on specialized agents capable of detecting, separating, and transcribing melodic and harmonic lines of instruments and vocals contained in audio recordings.

## 📂 Project Structure

- `notebooks/`: exploration and experiment notebooks
- `scripts/`: transcription pipeline
- `agents/`: specialized agents per instrument
- `models/`: trained and development models
- `data/`: input and processed data
- `utils/`: helper functions
- `tests/`: unit tests

## 🧠 Technologies Being Studied

- Source Separation: **Demucs**, **Spleeter**
- Transcription: **BasicPitch**, **CREPE**, **Onsets and Frames**
- Libraries: `PyTorch`, `Librosa`, `pretty_midi`, `music21`

## 🔬 Roadmap

- [ ] Separate sources (voice, piano, guitar)
- [ ] Transcribe each source to MIDI
- [ ] Convert MIDI to sheet music
- [ ] Develop instrument-specific agents
- [ ] Evaluate using musical transcription metrics

## ⚙️ Installation

```bash
pip install -r requirements.txt
```

## 🗂️ Usage Example

```bash
python scripts/audio_to_midi.py --input data/raw/music.wav --output data/midi/music.mid
python scripts/midi_to_sheet.py --input data/midi/music.mid --output output/music.pdf
```
