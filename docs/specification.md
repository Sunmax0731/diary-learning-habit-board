# 仕様

        ## 対象レコード

        - `diaryEntry`
- `studyBlock`
- `habitTile`
- `shortcutPractice`

        ## 必須項目

        `title`, `date`, `nextAction`

        ## 警告項目

        `reflection`, `reviewDate`

        ## フロー

        1. 入力レコードを受け取る。
        2. `src/core/scenarioEngine.js` が必須項目と警告項目を評価する。
        3. `src/report/reportBuilder.js` が検証結果を集計する。
        4. `dist/validation-result.json` を release evidence の前提証跡にする。

        ## 保存方針

        日記本文と習慣ログを端末内に保存し、同期は行わない
