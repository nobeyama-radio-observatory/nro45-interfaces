# 観測指示書

観測者が作り、COSMOS のマネージャーが読み込んで各装置に命令を送るための、テキストのファイルの組です。

| 項目 | 内容 |
|---|---|
| 書く部品 | 観測指示書の作成ソフト（いまは nobs。台帳の `tool-obs-script`）。7BEE などでは、観測者が手で作る |
| 読む部品 | COSMOS のマネージャー（台帳の `sw-cosmos`） |
| 非公開の部分 | 命令を受けたマネージャーと各装置の Local Controller のあいだの通信と、命令の実行の手順。文書の所在は記録がない（nro-45m-control の [docs/interfaces.md](https://github.com/nobeyama-radio-observatory/nro-45m-control/blob/main/docs/interfaces.md) の②） |

作成ソフトを替えても、形式は変えない予定です（YATSUGATAKE-NRO45-sam45compat の [docs/cosmos/observation-flow.md](https://github.com/nobeyama-radio-observatory/YATSUGATAKE-NRO45-sam45compat/blob/main/docs/cosmos/observation-flow.md) の1）。この仕様は、nobs を作り直すときの契約になります。

## 版の一覧

| 版 | 別名（実装の名前） | 状態 | 適用の期間 | 書く製品 | 読む製品 | データの版の印 |
|---|---|---|---|---|---|---|
| [v1](v1.md) | obstable（`.start`、`.dat`） | 案 | 記録がない（少なくとも nobs 2.230904_public の出力、2026-11 の時点） | nobs | COSMOS のマネージャー | ない（作成ソフトの版をコメントに書くだけ）。形式の版の欄があるかは確認中 |
