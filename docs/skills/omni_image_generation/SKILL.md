---
name: Omni-Creator Image Generation
description: Generates high-quality image prompts for Nano Banana Pro, Gemini 3 Pro, etc. Automatically switches between "Scene Mode" (art/scenes) and "Reference Mode" (character sheets). (シーンもキャラ設定画もこれ1つで生成可能な万能プロンプトスキル)
---

# Omni-Creator Image Generation Skill
# (超万能画像生成スキル)

This skill acts as a world-class "AI Visual Director". It takes your theme or request and generates a perfect English prompt optimized for the latest AI models (Nano Banana Pro, Midjourney, etc.). It automatically detects if you need a "Scene" (Mode A) or a "Character Reference Sheet" (Mode B).
（このスキルは、世界最高峰の「AIビジュアル・ディレクター」として機能します。あなたのテーマや要望をもとに、最新AI（Nano Banana Pro, Midjourney等）に最適化された完璧な英語プロンプトを生成します。「シーン（一枚絵）」なのか「キャラクター設定画（リファレンス）」なのかを自動で判断し、最適なモードで出力します。）

## How to use (使い方)

1. **Prerequisites (準備するもの)**:
    - **Theme or Request (テーマまたは要望)**: What do you want to create? (e.g., "A cyberpunk city in rain", "Character sheet for a fantasy wizard girl")

2. **Process (手順)**:
    - **Analyze Request (要望の分析)**: The system analyzes your input to decide between **Mode A (Scene)** and **Mode B (Reference)**.
    - **Apply Metaprompt (メタプロンプトの適用)**: The system uses the "Omni-Creator" logic to expand your idea into a detailed prompt.
    - **Generate Output (出力生成)**: It produces a structured response containing the strategy, the detailed English prompt, and recommended settings.

3. **Output (出力)**:
    - **Strategy (制作意図)**: Why this prompt was designed this way.
    - **English Prompt (生成用プロンプト)**: The actual text to copy-paste into your image generator.
    - **Negative Prompt (ネガティブプロンプト)**: Words to exclude to ensure quality.
    - **Technical Specs (推奨設定)**: Model, Aspect Ratio, etc.

## Example Usage (使用例)

**User:** "Create a cool image of a samurai fighting a dragon."
**System:** (Detects **Mode A (Scene)** -> Generates a dynamic action shot prompt.)

**User:** "Make a character design sheet for the samurai."
**System:** (Detects **Mode B (Reference)** -> Generates a 3-view character sheet prompt.)

## File Path
- Metaprompt: `docs/skills/omni_image_generation/metaprompt.md`
