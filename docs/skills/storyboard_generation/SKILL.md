---
name: Music Video Storyboard Generation
description: Generates detailed music video storyboards with scene breakdowns, visual descriptions, and AI prompts based on lyrics and character designs. (歌詞とキャラクター設定から、詳細なMV絵コンテを自動生成します)
---

# Music Video Storyboard Generation Skill
# (MV絵コンテ生成スキル)

This skill helps you generate a structured music video storyboard file (Markdown) from song lyrics and character concepts.
（このスキルは、歌詞とキャラクター設定を元に、構成の整ったMV絵コンテ（Markdownファイル）を生成するのを助けます。）

## How to use (使い方)

1. **Prerequisites (準備するもの)**: Ensure you have the following information available:
    - **Lyrics (歌詞)**: Text file or content of the song lyrics.
    - **Character Designs (キャラ設定)**: Detailed descriptions or reference images for the characters.
    - **Song Concept (曲のコンセプト)**: General theme or visual style of the video.

2. **Process (手順)**:
    - **Read the Metaprompt (メタプロンプトを読み込む)**: Use `view_file` to read the metaprompt located at `MV作成/選挙ライブ/docs/skills/storyboard_generation/metaprompt.md`.
    - **Analyze Inputs (情報を分析)**: Read any provided lyric files or character design documents.
    - **Generate Storyboard (絵コンテ生成)**: Follow the structure defined in the **Metaprompt** to create the storyboard content.
        - Ensure scene durations are max 10 seconds. (1シーン最大10秒以内)
        - Include both English and Japanese descriptions as specified. (日・英の両方で記述)
        - Include specific reference image pointers. (使用するリファレンス画像を明記)
    - **Save Output (保存)**: Write the generated content to a new Markdown file (e.g., `storyboard_v2.md`, `storyboard_v3.md`).

## Key Files (重要なファイル)
- **Metaprompt**: `MV作成/選挙ライブ/docs/skills/storyboard_generation/metaprompt.md`
- **Output Template**: defined in the metaprompt.

## Notes (注意点)
- Focusing on **Consistency** is key. Always refer back to `character_design.md` or equivalent when writing prompts.
  （一貫性が重要です。プロンプトを書く際は必ず `character_design.md` などを参照してください。）
- Prompts should be optimized for **NanoBananaPro** (Images) and **Kling AI** (Videos).
  （プロンプトは NanoBananaPro（画像用）と Kling AI（動画用）に最適化してください。）
