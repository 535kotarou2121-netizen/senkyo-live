# AIプロンプト・ライブラリ (AI Prompt Library)

このドキュメントは、実証済みの効果的なプロンプトを蓄積する場所です。
**ルール：プロンプトは英語、説明は日本語**

---

## 🎵 音楽生成 (Music Generation / Suno AI)

### ジャンル・スタイル (Genre & Style)
**Epic Orchestral / 壮大なオーケストラ**
```text
Epic Orchestral, Cinematic, Hollywood Soundtrack, Powerful Brass, Dramatic Strings, Choir, Hans Zimmer style, Emotional, Build up
```
*解説: 映画のクライマックスや演説シーンで使用。徐々に盛り上がる構成。*

**Heavy Metal / ヘヴィメタル**
```text
Heavy Metal, Aggressive, Fast Tempo, Double Bass Drum, Distorted Guitar, Growl Vocals, Male Vocals, Darkness, Power
```
*解説: 政治家の強い意志や怒りを表現する際に有効。*

**80s City Pop / 80年代シティポップ**
```text
80s City Pop, Japanese City Pop, Funk Bass, Synthesizer, Neon Lights feel, Groovy, Female Vocals, Nostalgic, Catchy
```
*解説: レトロで少しお洒落な雰囲気を出したい時（ギャップ狙い）。*

### 構造タグ (Structure Tags)
- `[Intro]`: イントロ
- `[Verse]`: Aメロ・Bメロ
- `[Chorus]`: サビ
- `[Bridge]`: 大サビ前の展開
- `[Build Up]`: 盛り上がりへの導入
- `[Outro]`: アウトロ
- `[End]`: 曲の終了
- `[Extended Fade]`: ゆっくりとしたフェードアウト

### ダイナミクスタグ (Dynamics Tags)
- `[Pianissimo]`: 非常に静かなパート
- `[Piano]`: 静かなパート
- `[Mezzo-forte]`: 中程度の音量
- `[Forte]`: 力強いパート
- `[Fortissimo]`: 非常に力強いパート
- `[Crescendo]`: 徐々に音量を上げる
- `[Decrescendo]`: 徐々に音量を下げる

### ボーカル強調テクニック (Vocal Emphasis)
- **大文字**: `FEEL THE POWER!` → ボーカルが力強く叫ぶように歌う
- **感嘆符**: `立ち上がれ!` → 感情的な強調
- **括弧**: `(Woah-oh-oh)` → バックボーカル/コーラス
- **[Spoken]**: `[Spoken] 誰にも止められない` → 語りパート

### サウンドエフェクト (Sound Effects)
- `*thunder cracking*` → 雷の効果音
- `*drum roll building*` → ドラムロール
- `*guitar shredding*` → ギターシュレッド
- `*crowd cheering*` → 歓声

### テンポ指定 (Tempo/BPM)
- `Fast Tempo 160 BPM` → 具体的なBPM指定（推奨）
- `Slow Tempo 70 BPM` → バラード向け
*解説: 数値でBPMを指定すると、より正確なテンポ制御が可能*

---

## 🇯🇵 日本語歌詞の最適化 (Japanese Lyrics Optimization)

Suno AIは漢字の読み間違いや、助詞「は」「へ」の発音ミス頻度が高いです。以下の対策を推奨します。

### 1. ひらがな・カタカナ化
漢字は極力使わず、ひらがなかカタカナに変換してください。
- ❌ `運命` → ⭕️ `うんめい` (Unmei)
- ❌ `明日` → ⭕️ `あした` (Ashita) ※「あす」と読まれるのを防ぐ

### 2. ローマ字併記 (Romanization)
確実に発音させるため、括弧書きでローマ字を添えると効果的です。特に助詞に有効です。
- `わたしは` → `わたしは (Watashi wa)`
- `えいえんへ` → `えいえんへ (Eien e)`

### 3. 空白によるリズム調整
言葉の間隔を空けることで、リズムを調整できます。
- `立ち上がれ` → `た ち あ が れ`

## 🖼️ 画像生成 (Image Generation / Midjourney, etc.)

### リアリズム・品質 (Realism & Quality)
**基本高品質セット**
```text
8k resolution, photorealistic, cinematic lighting, highly detailed, depth of field, sharp focus, shot on 35mm lens, f/1.8, realistic skin texture
```
*解説: 写真のようなリアルさを出すための必須呪文セット。アニメ調を避けるために重要。*

### 人物・政治家風 (Subject: Politician Style)
**演説中の政治家**
```text
Middle-aged Japanese male politician, wearing a formal dark suit and tie, speaking passionately at a podium, microphone, intense facial expression, hand gestures, blurred audience in background, news footage style
```
*解説: ニュース映像風の演説シーン。*

**シリアスな表情（クローズアップ）**
```text
Extreme close-up of a Japanese politician's face, serious expression, wrinkles, sweat drops, detailed eyes, intense gaze, dramatic side lighting, dark background
```
*解説: 苦悩や決意を表現する顔のアップ。*

### ネガティブプロンプト (Negative Prompts / 除外したい要素)
```text
cartoon, anime, illustration, painting, drawing, sketch, 3d render, watermark, text, signature, low quality, bad anatomy, deformed hands, extra fingers
```
*解説: イラストやCGっぽさを排除し、実写に近づけるための除外キーワード。*

---

## 🎥 動画生成 (Video Generation / Higgsfield, Runway)

### カメラワーク (Camera Movement)
**スローモーション**
```text
Slow motion, high frame rate, smooth movement
```
*解説: 重厚感を出すためによく使う。*

**ドローン視点**
```text
Drone shot, aerial view, establishing shot, wide angle, moving forward
```
*解説: 街頭演説の規模感や、街の様子を見せる時に使用。*

**ズームイン/アウト**
```text
Slow zoom in to face (顔へのゆっくりとしたズーム)
Pull back (引いていくカメラ)
```
*解説: 感情の変化や状況説明に。*
