# kakei — 家計簿 PWA

すばやく記録して、支出を見える化するブラウザ完結型の家計簿です。

## Features
- 店名 → ジャンル → 金額を入力して1タップ登録
- LocalStorageによるオフライン保存
- ジャンル別の支出分析・日別推移
- JSONバックアップ / 復元
- 共有リンク（URLハッシュにデータを埋め込む方式）
- ダーク / ライトテーマ
- Service Worker + Web App ManifestによるPWA
- GitHub Pagesで静的ホスティング可能

## Data model
支出は `{ id, store, category, amount, date, createdAt }` として端末内に保存します。

## Privacy
データはデフォルトではブラウザ内だけに保存されます。共有を実行した場合のみ、データをURLに含めて相手へ渡します。個人情報などを共有リンクに含めないでください。
