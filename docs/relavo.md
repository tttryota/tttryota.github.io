#　コンセプト
タグ方式で体験を記録し、スコアベースのランキングによる相対評価で価値観を磨くアプリ。
物事の評価は自身の過去との比較によって実現され、その行為の繰り返すことで価値観を明らかにする。

# なぜ作ったか
以下を同時に実現するサービスが存在せず、ニッチながらもペインがあると判断したから（ただしターゲットは絞り切れていない）
- 体験を記録する
- タグで整理する
- 固定ではなく柔軟なランキングを生成する
 
# 特徴
- ユーザーの「こうなるだろう」を裏切らない操作感
- コンセプトを体現したUX
  - スコアは過去の評価を可視化した上で決定できる
- ゲーミフィケーション要素（記録数に応じたバッジ獲得）で記録作成のモチベーション維持

# 技術スタック
## Mobile
- React Native 0.81 / Expo 54
- Tamagui
- Jotai
- TanStack Query
- React Native IAP
- Sentry
- Google Sign-In / Apple Auth

## Backend
- Django 4.2 / DRF
- PostgreSQL (Neon)
- JWT Auth (SimpleJWT)
- Cloudflare R2 (boto3経由)
- Sentry
- Gunicorn
- Render (ホスティング)

