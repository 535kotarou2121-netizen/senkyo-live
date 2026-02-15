---
description: 新しいMVプロジェクトの立ち上げと構成案の作成プロセス
---

1. **ヒアリング (Requirements Gathering)**
   - 以下の情報をユーザーに確認する:
     - 楽曲タイトル (Title) 〜 決まっていなければ仮タイトル
     - ジャンル (Genre) 〜 例: Heavy Metal, City Pop
     - コンセプト/テーマ (Concept) 〜 映像の雰囲気やストーリー
     - バンドメンバーと担当楽器 (Band Members) 〜 誰が何を演奏するか

2. **プロジェクトディレクトリ作成 (Project Setup)**
   - プロジェクト名から英語のスラッグを決定 (例: `iron_coalition`)
   // turbo
   - ディレクトリ作成コマンドを実行: `mkdir -p projects/[slug]`
   - `.gitignore` の確認・更新:
     - プロジェクトルートの `.gitignore` に `*.mp3` が含まれているか確認し、なければ追加する。
     - 生成された音楽ファイルがGit管理下に入らないようにするため。

3. **リソース読み込み (Load Resources)**
   - 以下のファイルを `view_file` で読み込む:
     - `docs/MV_Storyboard_Template.md` (構成案テンプレート)
     - `docs/Prompt_Library.md` (プロンプト集)
     - `docs/skills/prompt_guidelines.md` (プロンプト作成ルール)

4. **構成案の作成 (Draft Storyboard)**
   - 収集した情報とテンプレートを元に、`projects/[slug]/mv_storyboard.md` を作成する
   - **重要ルール**:
     - プロンプトは**英語**、解説は**日本語**
     - 画質設定は `8k resolution, photorealistic` 等を含める (Prompt Library参照)
     - シーン構成は標準10シーン (Intro, Verse, Chorus, Solo, Outro等)
     - 歌詞案も同時に作成する (日本語/英語ミックス等)

5. **レビューと修正 (Review)**
   - ユーザーに作成したファイルを確認してもらう
   - 修正があれば反映する
