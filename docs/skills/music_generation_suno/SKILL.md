---
name: music_generation_suno
description: Suno AIを使用した音楽生成のためのプロンプトとテクニック
---

# 🎵 Music Generation (Suno AI)

Suno AIを使って高品質な楽曲を生成するためのプロンプト集です。

## 発動条件 (Triggers)
**以下の文脈・依頼があった場合、このスキルのプロンプトを使用してください。**
1. **楽曲生成依頼**: 「曲を作りたい」「BGMを作って」「Sunoで生成する」
2. **プロンプト作成**: 「Sunoのプロンプトを考えて」「スタイルはどうすればいい？」
3. **歌詞・構成**: 「歌詞ができたから曲にしたい」（`optimize_suno_lyrics` と併用推奨）

---

## ジャンル・スタイル (Genre & Style)

### Epic Orchestral / 壮大なオーケストラ
```text
Epic Orchestral, Cinematic, Hollywood Soundtrack, Powerful Brass, Dramatic Strings, Choir, Hans Zimmer style, Emotional, Build up
```
*解説: 映画のクライマックスや演説シーンで使用。徐々に盛り上がる構成。*

### Heavy Metal / ヘヴィメタル
```text
Heavy Metal, Aggressive, Fast Tempo, Double Bass Drum, Distorted Guitar, Growl Vocals, Male Vocals, Darkness, Power
```
*解説: 政治家の強い意志や怒りを表現する際に有効。*

### 80s City Pop / 80年代シティポップ
```text
80s City Pop, Japanese City Pop, Funk Bass, Synthesizer, Neon Lights feel, Groovy, Female Vocals, Nostalgic, Catchy
```
*解説: レトロで少しお洒落な雰囲気を出したい時（ギャップ狙い）。*

---

## 構造・構成 (Structure & Dynamics)

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
- `[Fortissimo]`: 非常に力強いパート
- `[Crescendo]`: 徐々に音量を上げる

### ボーカル強調 (Vocal Emphasis)
- **大文字**: `FEEL THE POWER!` → 力強く叫ぶ
- **感嘆符**: `立ち上がれ!` → 感情的強調
- **括弧**: `(Woah-oh-oh)` → バックボーカル
- **Spoken**: `[Spoken] 語り`

### サウンドエフェクト (Sound Effects)
- `*thunder cracking*` (雷)
- `*drum roll building*` (ドラムロール)
- `*guitar shredding*` (ギターソロ)
- `*crowd cheering*` (歓声)

### テンポ指定 (Tempo/BPM)
- `Fast Tempo 160 BPM` (推奨: 数値指定)
- `Slow Tempo 70 BPM`

---

## 🇯🇵 日本語歌詞の最適化 (Japanese Lyrics Optimization)
Suno AIの読み間違いを防ぐためのテクニックです。

1. **ひらがな・カタカナ化**: 漢字は使わず、ひらがなにする。
   - `運命` → `うんめい`
2. **ローマ字併記**: 助詞はローマ字で補助。
   - `わたしは` → `わたしは (Watashi wa)`
3. **リズム調整**: 空白を入れる。
   - `た ち あ が れ`
