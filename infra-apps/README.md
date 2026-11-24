# インフラ実務ミニアプリ集

インフラ・ネットワークの学習や検証で使える小さなアプリです。各アプリの `index.html` をダウンロードしてブラウザーで開くと使えます。外部ライブラリ、APIキー、サーバーは不要です。SHA-256照合でブラウザーがローカルファイルの暗号化機能を制限する場合は、localhostまたはHTTPSで開いてください。

| アプリ | できること | ファイル |
| --- | --- | --- |
| IPv4 サブネット計算 | CIDRからサブネットマスク、利用可能なIP範囲、ホスト数を算出。/31はポイントツーポイント、/32は単一ホストとして扱います。 | [index.html](subnet-calculator/index.html) |
| 障害対応タイムライン | 検知・調査・復旧・連絡のメモを時刻順に整列し、テキストで出力。ページを閉じる前に保存してください。 | [index.html](incident-timeline/index.html) |
| バックアップ容量見積もり | フル1回と日次増分の合計に余裕分を加えて、必要容量を算出。 | [index.html](storage-estimator/index.html) |
| ログ絞り込み | 貼り付けたログからキーワードを含む行と、その前後の行を行番号付きで抽出します。 | [index.html](log-slicer/index.html) |
| Unix時刻変換 | Unix時刻の秒・ミリ秒と、UTC・日本時間を相互に確認できます。日時から変換するときはタイムゾーンも入力します。 | [index.html](epoch-converter/index.html) |
| JSON差分比較 | 設定やAPI応答を比較し、追加・削除・変更があった位置をJSON Pointerで表示します。オブジェクトのキー順は無視します。 | [index.html](json-diff/index.html) |
| ファイルのSHA-256照合 | ファイルのSHA-256を端末内で計算し、配布元が示したハッシュ値と照合します。上限は64 MiBです。 | [index.html](file-checksum/index.html) |
| 予定の重複チェック | 同じ日の勤務・授業・面接などの予定を入力し、時間が重なる組み合わせを確認できます。 | [index.html](schedule-overlap/index.html) |
