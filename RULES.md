# メカニカ外部設定資料：運用ルール

## 参照リポジトリ

メカニカ外部設定資料として参照するGitHubリポジトリは、原則として以下のみとする。

```text
Tororomochi/meccanica
https://github.com/Tororomochi/meccanica
```

## 基本運用

- 「GitHubの設定を見る」「該当mdを参照する」「外部設定資料を呼び出す」と言われた場合、このリポジトリを優先して参照する。
- 本編データはこのリポジトリへ置かない。
- このリポジトリは、メカニカの外部作品クロスオーバー設定資料として使う。
- Blue Archive関連の学校、組織、キャラクター、メカニカとの関係性を整理する。
- 公式設定は要約に留め、丸写ししない。
- メカニカとの関係、運用、認知レベルを中心に記録する。

## キャラクター検索

- Blue Archive系キャラクターを探す場合は、まず `character-index.md` を参照する。
- `character-index.md` は、キャラクター名から該当Markdownファイルへ辿るための索引として扱う。
- キャラクター個別設定の詳細は、`character-index.md` に記載されたリンク先の各Markdownを参照する。
- 新しいキャラクター資料を追加した場合は、必要に応じて `character-index.md` にも追記する。

## Blue Archive Story運用

- Blue Archive側ストーリーを書く、続きを作る、直近の流れを確認する場合は、開始前に必ず `crossover/blue-archive/story/timestamp.md` を参照する。
- `timestamp.md` では数字が大きいほど新しいストーリーとして扱う。
- 続きを書く場合や直近の流れを確認する場合は、最新番号の章ファイルと、その1つ前の章ファイルを読む。
- 全体時系列を確認する場合は、`crossover/blue-archive/story/timeline.md` の運用方針とタイムラインも参照する。
- `timeline.md` は物語上の順番を管理するファイルであり、各 `Txx` には対応する章ファイルを関連資料として記載する。

## 「あらすじをアップ」運用

- ユーザーが「あらすじをアップ」「あらすじを上げて」「あらすじを追加して」と言った場合は、渡されたあらすじを `crossover/blue-archive/story/` 配下へ番号付きMarkdownとして追加する。
- ファイル名は `04-english-slug.md` のように、次の連番2桁 + 英語スラッグで作成する。
- 日本語の `あらすじ.md` や無番号ファイル名では保存しない。
- 追加後は `timestamp.md` に新しい番号、ファイル名、主題、状態を追記する。
- 必要に応じて `timeline.md` に新しい `Txx` を追加し、関連資料へ新章ファイルを記載する。
- 必要に応じて `README.md` のStory一覧にも追加する。
- 既に無番号の `あらすじ.md` が存在する場合は、内容に合う番号付き英語スラッグへ移し、旧ファイルは削除する。

## 重要ルール

- アロナとプラナは先生以外には基本的に認識できない。
- 先生はメカニカをまず生徒として扱う。
- 救護騎士団とシスターフッドはメカニカのことを知らない。
- メカニカは人間相手にはノーキル方針を維持する。

## 主な参照先

```text
character-index.md
crossover/blue-archive/story/timestamp.md
crossover/blue-archive/story/timeline.md
crossover/blue-archive/schools.md
crossover/blue-archive/schale/
crossover/blue-archive/general-student-council/
crossover/blue-archive/millennium/
crossover/blue-archive/trinity/
crossover/blue-archive/gehenna/
crossover/blue-archive/abydos/
```
