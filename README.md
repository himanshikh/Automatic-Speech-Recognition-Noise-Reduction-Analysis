# 🎙️ ASR Noise Reduction & Word Error Rate (WER) Evaluation

## 📌 Overview

This project investigates how noise reduction techniques improve the performance of an Automatic Speech Recognition (ASR) system.

The experiment evaluates transcription accuracy before and after applying noise suppression and measures performance using **Word Error Rate (WER)**.

**Reference Sentence Used:**

> "The quick brown fox jumps over the lazy dog."

---

##  Objective

- Record clean and noisy speech samples
- Apply noise reduction to the noisy audio
- Transcribe all audio samples using an ASR engine
- Evaluate transcription accuracy using Word Error Rate (WER)
- Compare noisy vs. denoised ASR performance

---

##  Tech Stack

- Python
- SciPy
- Noisereduce
- SpeechRecognition
- JiWER
- SoundDevice

---


## Installation

Install the required libraries:

scipy noisereduce speechrecognition jiwer sounddevice

---

## Methodology
1️ Audio Recording

Two separate recordings were created:

Clean recording (quiet environment)

Noisy recording (background noise introduced intentionally)

2️ Noise Reduction

Applied spectral gating-based noise reduction using the noisereduce library.

Generated a cleaned audio file from the noisy recording.

3️ Transcription

Converted speech to text using the SpeechRecognition library.

Generated transcripts for:

Clean audio

Noisy audio

Denoised audio

4️ Evaluation

Used the jiwer library to compute Word Error Rate (WER).

Compared WER between noisy and cleaned audio.
