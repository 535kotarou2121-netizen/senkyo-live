---
name: Character Reference Generation
description: Generates a prompt to create a consistent character reference sheet (Reference Image) for AI image generation. (AI画像生成用の一貫したキャラクターリファレンスシートを作成するためのプロンプトを生成します)
---

# Character Reference Generation Skill
# (キャラクターリファレンス生成スキル)

This skill generates a prompt to create a "Master Reference Image" that fixes the character's identity (face, bone structure, features). This reference image is essential for maintaining consistency in subsequent generations (Identity Locking).
（このスキルは、キャラクターのアイデンティティ（顔立ち、骨格、特徴）を固定した「マスターリファレンス画像」を作成するためのプロンプトを生成します。このリファレンス画像は、後の生成で一貫性を保つ（アイデンティティ・ロッキング）ために不可欠です。）

## How to use (使い方)

1. **Prerequisites (準備するもの)**:
    - **Character Settings (キャラクター設定)**: A description of the character you want to create (age, gender, appearance, style, etc.).

2. **Process (手順)**:
    - **Read Metaprompt (メタプロンプトの読み込み)**: The system reads the `metaprompt.md` file.
    - **Input Settings (設定の入力)**: Provide the character settings to the system.
    - **Generate Prompt (プロンプト生成)**: The system generates a prompt for the AI image generator (Nano Banana Pro, Midjourney, etc.) based on the metaprompt.

3. **Output (出力)**:
    - **Generation Strategy (生成方針)**: Explanation of the approach.
    - **Prompt (プロンプト)**: The actual prompt to use for image generation.
    - **Negative Prompt (ネガティブプロンプト)**: Words to exclude.

## Example Usage (使用例)

**User:** "Generate a reference sheet for a cyberpunk female hacker, asian, purple hair, neon jacket."

**System:** (Reads `metaprompt.md`, inserts the settings, and outputs the detailed prompt.)

## File Path
- Metaprompt: `docs/skills/character_reference_generation/metaprompt.md`
