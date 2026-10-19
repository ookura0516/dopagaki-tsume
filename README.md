# dopagaki-tsume

「ドパガキ将棋」の追加詰将棋問題の配信用リポジトリです。アプリは jsDelivr 経由で読み込みます。

- `packs/index.json`：`{"packs":["pack-001.json", ...]}`
- `packs/pack-NNN.json`：同梱問題と同じ形式（`{"version":1,"pack":"pack-NNN","problems":[...]}`）

問題は `dopa_engine` の `bin/tsume_gen.dart` で作り、`bin/tsume_verify.dart` で全問の唯一解を確かめてから追加します。
