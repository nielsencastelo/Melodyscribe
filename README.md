# Melodyscribe 🎼🤖

**Status: Em desenvolvimento.** 🚧

Melodyscribe é um sistema baseado em Inteligência Artificial para transcrição automática de músicas (WAV, MP3) em partituras em formato PDF, com suporte a múltiplos instrumentos e voz.

## 🎯 Objetivo

Criar uma ferramenta colaborativa baseada em agentes especializados que possam detectar, separar e transcrever linhas melódicas e harmônicas de instrumentos e vozes contidos em gravações de áudio.

## 📂 Estrutura do Projeto

- `notebooks/`: notebooks com explorações e experimentos
- `scripts/`: pipeline de transcrição
- `agents/`: agentes por instrumento
- `models/`: modelos treinados e salvos
- `data/`: dados de entrada e processados
- `utils/`: funções auxiliares
- `tests/`: testes unitários

## 🧠 Tecnologias em Estudo

- Separadores: **Demucs**, **Spleeter**
- Transcrição: **BasicPitch**, **CREPE**, **Onsets and Frames**
- Libs: `PyTorch`, `Librosa`, `pretty_midi`, `music21`

## 🔬 Roadmap

- [ ] Separar fontes (voz, piano, guitarra)
- [ ] Transcrição MIDI de cada fonte
- [ ] Conversão MIDI → Partitura
- [ ] Agentes especializados por instrumento
- [ ] Avaliação com métricas musicais

## ⚙️ Instalação

```bash
pip install -r requirements.txt
```

## 🗂️ Exemplo de Uso

```bash
python scripts/audio_to_midi.py --input data/raw/music.wav --output data/midi/music.mid
python scripts/midi_to_sheet.py --input data/midi/music.mid --output output/music.pdf
```
