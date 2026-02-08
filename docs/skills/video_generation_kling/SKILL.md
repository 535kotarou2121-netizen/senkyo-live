---
name: video_generation_kling
description: Kling, Runway等を使用した動画生成のためのカメラワークプロンプト
---

# 🎥 Video Generation (Kling, Runway, Higgsfield)

静止画を動画化する際や、動画生成AIを使うためのカメラワーク指示集です。

## 発動条件 (Triggers)
**以下の文脈・依頼があった場合、このスキルのプロンプトを使用してください。**
1. **動画化依頼**: 「この画像を動かしたい」「動画を作って」「Klingで生成する」
2. **カメラワーク**: 「ズームインさせたい」「ドローンで撮ったようにしたい」
3. **動きの指定**: 「スローモーションにして」「風でなびかせて」

---

## カメラワーク (Camera Movement)

### スローモーション (Slow Motion)
```text
Slow motion, high frame rate, smooth movement
```
*解説: 重厚感を出すためによく使う。*

### ドローン視点 (Drone Shot)
```text
Drone shot, aerial view, establishing shot, wide angle, moving forward
```
*解説: 街頭演説の規模感や、街の様子を見せる時に使用。*

### ズームイン/アウト (Zoom)
- **Zoom In**: `Slow zoom in to face` (顔へのゆっくりとしたズーム)
- **Pull Back**: `Pull back`, `Zoom out` (引いていくカメラ)
*解説: 感情の変化や状況説明に。*

---

## AIツール別ヒント

### Kling AI
- **Motion Brush**: 特定の箇所（手や旗など）だけを動かしたい場合に使用。
- **Camera Control**: Pan, Tilt, Zoomの数値を細かく調整可能。

### Runway Gen-2/Gen-3
- **Motion Brush**: 複数のブラシを使って動きを制御できる。
