# 🎵 Omnizart Colab Fixed (2026.01 Edition)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](請貼上你的Colab網址)
![Status](https://img.shields.io/badge/Status-Fixed-green)
![Python](https://img.shields.io/badge/Python-3.8-blue)

這是一個經過修復的 **Omnizart** Google Colab 版本。
This is a fixed and working version of **Omnizart** for Google Colab.

原版 Omnizart 在 2026 年的 Colab 環境中因為相依性套件（如 Python 版本、Librosa、Spleeter）升級而無法直接執行。本專案解決了這些環境衝突。
The original Omnizart notebook fails in 2025 due to dependency conflicts (Python version, Librosa, Spleeter). This project fixes those "Dependency Hell" issues.

---

## 🛠️ 修復內容 (What's Fixed)

在此版本中，我們解決了以下問題：
We have resolved the following issues:

1.  **Python 環境 (Environment)**：
    - 強制使用 **Python 3.8** (透過 Miniforge)，解決 Colab 預設 Python 3.10/3.11 不相容的問題。
    - Enforced **Python 3.8** via Miniforge to fix incompatibility with Colab's default Python 3.10/3.11.

2.  **相依性衝突 (Dependencies)**：
    - 鎖定 `librosa==0.8.0` 與 `numba==0.53.0` 以支援 Spleeter。
    - Pinned `librosa==0.8.0` and `numba==0.53.0` to support Spleeter.

3.  **CLI 錯誤 (CLI Errors)**：
    - 修復 `tqdm` 版本錯誤導致的 `ModuleNotFoundError`。
    - Fixed `ModuleNotFoundError` caused by `tqdm` version mismatch.
    - 修復 `pretty_midi` 與 `pyfluidsynth` 遺失的問題。
    - Fixed missing `pretty_midi` and `pyfluidsynth` packages.

---

## 🙏 致謝 (Credits)

本專案是 **Omnizart** 的非官方修復版本。
This project is an unofficial wrapper/fix for **Omnizart**.
**Original Project**: [Music-and-Culture-Technology-Lab/omnizart](https://github.com/Music-and-Culture-Technology-Lab/omnizart)
