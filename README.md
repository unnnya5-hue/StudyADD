# AI駆動開発 体験デモ

選択肢からAIに指示を出すだけで、**要件定義 → 実装 → テスト仕様書 → 打鍵テスト → バグ修正・回帰テスト**までを体験できるデモサイトです。
題材は「チームTODO」アプリです。

- `index.html` 1ファイルで完結しています（外部ライブラリ・CDN・通信なし）
- 演出は台本どおりの一本道で、選択肢によってAIの返答が少し変わります
- 打鍵テストは、完成したアプリをプレビュー上で実際に自動操作して判定しています（初回は2件NGになり、修正後に全件OKになります）

## 使い方

| 操作 | 内容 |
|---|---|
| `1` / `2` キー、またはクリック | 選択肢を選ぶ |
| `Space` / `→` / ⏭ スキップ | 次の選択肢まで演出を早送り |
| 右上の 1x / 2x / 4x | 演出の速度 |
| ↺ 最初から | リセット |

推奨：PCの Chrome / Edge、横幅1280px以上。プロジェクターで小さく見える場合はブラウザの拡大（Ctrl +）で調整してください。

## GitHub Pages で公開する手順

1. GitHub で新しいリポジトリを作成（例：`ai-dev-demo`）
2. このリポジトリを push
   ```sh
   git remote add origin https://github.com/<ユーザー名>/ai-dev-demo.git
   git push -u origin snailfish:main
   ```
3. GitHub のリポジトリ画面 → **Settings → Pages**
4. 「Build and deployment」の Source を **Deploy from a branch**、Branch を **main / (root)** にして Save
5. 1〜2分後に `https://<ユーザー名>.github.io/ai-dev-demo/` で開けるようになります

※ GitHub Pages の公開URLは誰でも閲覧できます（無料プランではリポジトリもPublicにする必要があります）。社外秘の情報は含めないでください。
