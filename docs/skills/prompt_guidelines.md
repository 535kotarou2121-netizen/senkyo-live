# スキル：プロンプト生成ガイドライン (Prompt Generation Guidelines)

このドキュメントは、AIプロジェクトにおけるプロンプト生成のルールを定義したものです。
今後新しいルールが追加された場合は、このファイルを更新してください。

## 1. 基本出力ルール (Core Output Rules)

**「プロンプトは英語、説明は日本語」**

AIツール（Suno, Midjourney, Higgsfield, Video AIなど）に入力するプロンプトは、精度を高めるために**必ず英語**で記述してください。
そのプロンプトがどのような意図で作られたか、どの部分が重要かを**日本語で**別枠に記載してください。

### フォーマット例 (Format Example)

**プロンプト (Prompt):**
```markdown
Cinematic shot, intense close-up of a Japanese politician giving a speech in heavy rain, dramatic lighting, high contrast, 8k resolution, photorealistic, emotional expression, raindrops on face, dark suit, blurred crowd in background
```

**解説 (Explanation):**
- **Cinematic shot, intense close-up**: 映画のような迫力と、被写体の感情を強調するためのクローズアップ指定。
- **Heavy rain, raindrops on face**: ドラマチックな演出を加えるための環境設定。
- **Dark suit, blurred crowd**: 主役（政治家）を際立たせるための服装と背景のボケ味。

---

## 2. 各AIツール別 ポイント (Tool-Specific Tips)

※ここに各ツールごとの特有のテクニックを追記していきます。

### Suno AI (Music)
- **Style Prompts**: 英語でジャンル、楽器、雰囲気を指定（例: `Heavy Metal, Aggressive Guitar, Male Vocals, Fast Tempo`）。
- **Lyrics**: 日本語の歌詞を使用する場合でも、[Verse], [Chorus] などの構造タグは英語で記述。

### Image/Video Generation (Midjourney, Higgsfield, etc.)
- **Quality Tags**: `statue`, `painting` 等のスタイルが混ざらないよう、`photorealistic`, `4k` 等を明記。
- **Negative Prompts**: 不要な要素（例: `cartoon`, `anime`, `illustration`）を除外する指示を含める。
