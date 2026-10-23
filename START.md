# START

このファイルは、`Tororomochi/meccanica` リポジトリを扱う時の入口である。

新しいチャットや別スレッドで `同期スタート` と言われた場合は、まずこのファイルを読み、ここに書かれた順番で必要資料を確認してから作業を開始する。

---

## 起動コマンド

### 同期スタート

`同期スタート` は、このリポジトリの作業開始コマンドとして扱う。

実施内容:

1. `START.md` を読む。
2. `RULES.md` を読む。
3. 必要に応じて `rule.md` も読む。
4. 作業内容に応じて、下記の参照先を読む。
5. 読み込んだルールと既存資料に従って作業する。

---

## 基本参照

リポジトリ全体を扱う場合、まず以下を参照する。

```text
README.md
RULES.md
START.md
```

補助的に旧ルール・原本ルールを確認する場合:

```text
rule.md
```

---

## キャラクター検索

キャラクターを探す場合は、まず以下を参照する。

```text
character-index.md
```

運用:

- Blue Archive系キャラクターを探す時は、個別ディレクトリを直接探し回る前に `character-index.md` を見る。
- `character-index.md` でキャラクター名から該当Markdownへ移動する。
- 新キャラクター資料を追加した場合は、必要に応じて `character-index.md` も更新する。

---

## Blue Archiveストーリー作業

Blue Archive側ストーリーを書く、続きを作る、あらすじを追加する、直近の流れを確認する場合は、以下の順で読む。

```text
crossover/blue-archive/story/timestamp.md
最新番号の章ファイル
最新番号の一つ前の章ファイル
crossover/blue-archive/story/timeline.md
```

運用:

- `timestamp.md` では数字が大きいほど新しいストーリーとして扱う。
- 続きを書く場合は、最新章と一つ前の章を必ず読む。
- 全体の流れや章の位置づけを確認する場合は `timeline.md` も読む。
- `timeline.md` の運用方針に従い、物語上の順番は `Txx` で管理する。

---

## Azur Laneストーリー作業

Azur Lane側ストーリーを書く、続きを作る、あらすじを追加する、直近の流れを確認する場合は、以下の順で読む。

```text
crossover/azur-lane/story/timestamp.md
最新番号の章ファイル
最新番号の一つ前の章ファイル（存在する場合）
crossover/azur-lane/story/timeline.md
```

運用:

- Blue Archive側とは別系統のストーリーとして扱い、章・時系列・同期地点を混在させない。
- `timestamp.md` では数字が大きいほど新しいAzur Lane側ストーリーとして扱う。
- 続きを書く場合は最新章を必ず読み、二章以上存在する場合は一つ前の章も読む。
- 全体の流れや章の位置づけを確認する場合は `timeline.md` も読む。
- Azur Lane側で副官と副司令官は別職として扱う。副官は秘書・事務補佐、副司令官は正式な指揮系統と代行権を持つ役職とする。
- 指揮系統や基地運用は、Azur Lane側ではリアル軍制寄りの運用を優先する。

### Azur Lane側同期

ユーザーが以下のように指定した場合は、Azur Lane側だけを同期対象として扱う。

```text
アズールレーン側を同期
アズレン側を同期
Azur Lane側を同期
```

実施内容:

1. `START.md` と `RULES.md` を読む。
2. `crossover/azur-lane/story/timestamp.md` を読む。
3. 最新章を読む。
4. 二章以上存在する場合は一つ前の章も読む。
5. 必要に応じて `crossover/azur-lane/story/timeline.md` を読む。
6. Blue Archive側の章・timestamp・timelineは変更しない。
7. Azur Lane側だけで続きを作成・同期する。

---

## あらすじアップ

ユーザーが以下のように言った場合は、あらすじ追加作業として扱う。

```text
あらすじをアップ
あらすじを上げて
あらすじを追加して
```

実施内容:

1. `START.md` を読む。
2. `RULES.md` を読む。
3. `crossover/blue-archive/story/timestamp.md` を読む。
4. 最新章と一つ前の章を読む。
5. 必要に応じて `timeline.md` を読む。
6. 新しいあらすじを次の連番で保存する。
7. `timestamp.md` を更新する。
8. 必要に応じて `timeline.md` に新しい `Txx` を追加する。
9. 必要に応じて `README.md` のStory一覧を更新する。

ファイル名ルール:

```text
04-english-slug.md
05-english-slug.md
06-english-slug.md
```

- 2桁以上の連番 + 英語スラッグで保存する。
- 日本語名の `あらすじ.md` や無番号ファイル名では保存しない。
- 既に `あらすじ.md` のような無番号ファイルがある場合は、内容に合う番号付き英語スラッグへ移し、旧ファイルは削除する。

### Azur Lane側あらすじアップ

ユーザーがAzur Lane側を明示してあらすじ追加を依頼した場合は、Blue Archive側ではなく以下を更新する。

```text
crossover/azur-lane/story/
```

実施内容:

1. `crossover/azur-lane/story/timestamp.md` を読む。
2. 最新章を読む。
3. 二章以上存在する場合は一つ前の章も読む。
4. 必要に応じて `crossover/azur-lane/story/timeline.md` を読む。
5. 新しいあらすじを次の連番 + 英語スラッグで保存する。
6. Azur Lane側の `timestamp.md` を更新する。
7. 必要に応じてAzur Lane側の `timeline.md` を更新する。
8. 必要に応じて `README.md` のStory一覧を更新する。
9. Blue Archive側のstoryファイルは変更しない。

---

## README更新

以下の場合は、必要に応じて `README.md` を更新する。

- 新しい章ファイルを追加した。
- 新しい学校・組織・カテゴリを追加した。
- ルート直下に重要ファイルを追加した。
- 新しい索引ファイルを追加した。

`START.md` 自体を追加・更新した場合も、必要に応じて `README.md` のルート構成へ反映する。

---

## ルール更新

運用ルールを追加・変更した場合は、基本的に以下へ反映する。

```text
RULES.md
```

必要に応じて、旧ルール参照用の以下にも同内容を追記する。

```text
rule.md
```

---

## よく使うエイリアス

### 同期スタート

リポジトリ作業の入口。

- `START.md` を読む。
- 作業内容に応じて必要資料を読む。
- ルールに従って作業を開始する。

### あらすじアップ

新しいBlue Archiveストーリー章を番号付きMarkdownとして追加する。

- 新章ファイル作成
- `timestamp.md` 更新
- `timeline.md` 更新
- `README.md` 更新

### アズールレーン側を同期

Azur Lane側だけを同期する。

- `crossover/azur-lane/story/timestamp.md` を読む。
- 最新章を読む。
- 必要に応じて一つ前の章と `timeline.md` を読む。
- Blue Archive側を変更しない。

### Azur Lane側あらすじアップ

新しいAzur Laneストーリー章を番号付きMarkdownとして追加する。

- Azur Lane側の新章ファイル作成
- Azur Lane側 `timestamp.md` 更新
- Azur Lane側 `timeline.md` 更新
- 必要に応じて `README.md` 更新
- Blue Archive側は変更しない

### キャラ同期

キャラクター索引の更新作業。

- 新キャラや新規キャラ資料を確認する。
- `character-index.md` に追記する。
- 必要に応じて `README.md` も更新する。

---

## 禁止・注意

- 公開GitHubに本編核心情報、原初情報、年齢、旧素性、帰還事故、2025年関連情報を直接書かない。
- 公式設定は丸写ししない。要約とクロスオーバー運用に留める。
- Blue Archive側では、メカニカはミレニアムの短期編入生・ゲーム開発部の新人として扱う。
- アロナとプラナは先生以外には基本的に認識できない。
- メカニカは人間相手にはノーキル方針を維持する。
