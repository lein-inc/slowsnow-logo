# slow snow STUDIO — ロゴ提案サイト

staticrypt でパスワード暗号化した静的ページ。PDF・音源は暗号化 HTML 内に埋め込み（平文ファイルは置かない）。

再ビルド: `src/*.html` を編集 → `npx staticrypt src/<name>.html -p '<password>' --short --remember 30 -d .` → 日本語 UI 置換（CHANGELOG 参照）。
