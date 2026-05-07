# diary-learning-habit-board

日記・学習・習慣ボード は、日記、学習、習慣タイルを日単位で確認するローカルボードです。

## Closed Alpha Scope

- Rank: 22
- Tier / Score: P1 / 65
- Domain / Idea No: WindowsApp / 9
- 主な公開先: GitHub Release / BOOTH
- GitHub: https://github.com/Sunmax0731/diary-learning-habit-board
- Prerelease: https://github.com/Sunmax0731/diary-learning-habit-board/releases/tag/v0.1.0-alpha.1

## 実装概要

- `src/core`: 製品プロファイルと代表シナリオ評価
- `src/validators`: 期待結果検証
- `src/report`: 検証レポート生成
- `src/review-model`: レビューゲートと責務モデル
- `src/cli`: `samples/representative-suite.json` の自動検証

## 代表データ

`samples/representative-suite.json` は `happy-path`、`missing-required`、`warning`、`mixed-batch` を含みます。

## 検証

```powershell
cd D:\AI\WindowsApp\diary-learning-habit-board
cmd.exe /d /s /c npm test
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` を参照してください。
